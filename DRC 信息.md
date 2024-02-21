---

title: DRC 信息
tags: [DRC, layer, Edge, polygon]
date created: 星期三, 一月 3日 2024, 2:50:52 下午
date modified: 星期三, 二月 21日 2024, 2:35:54 下午
---

#DRC #layer #Edge #polygon 
## Layers的导入

- DRC layers input psu.set_input_layout： 将一个具体的GDS文件和我们命名的layout_handler相关联。 pu.get_input_layout_handle 通过名字获取返回某一层， 从而实现得到版图某一层读取
- layers output 方式与input类似
- set Patch size : 通过 psu.set_patch_size(patch_size) 设置分片正方形的大小 单位是微米
- Set DBU: psu.set_dbu(num) 设置优化过程中数据处理的最小单位
- Set boundary handing at global level 设置周边分块对自身的影响 psu.set_boundary_handling(1,option{}) 第一个参数 0 表示每个分片单独优化不考虑边界影响，1表示考虑边界影响。
## [[Polygon]]
## [[Edge]]
## [[vertex]]

## [[Polygon#Polygon 的选择|Polygon的选择]]
# [[Edge]] 的选择

## [[Edge]] Operations General

### Frequently-used [[edge]] Operation Commands Include:

- [[Mark]] commands
- [[Bias]] 
- [[Edge]] conversion commands
    - pu.convert_non90
    - pu.convert_non45
- Corner chop commands
    - pu.chop_corner
    - pu.chop_acute
- Corner / jog / notch / nub handling commands
    - pu.detete_corner_jog / pu.detect_notch_nub
    - pu.clear_corner_jog / pu.clear_notch_nub

### [[Edge]] Conversion Command

- pu.convert_non90/45 可以把任意角度的边转换为水平或竖直/45倍数的边
```python
general_setting = {'step_length’:8}
special_setting = []
options = {}
options['strict_mode'] = 'manhattan'
layer_design = pu.convert_non45(layer_main, general_setting, special_setting, options=options)
```
- options mode
	- auto ： 为原转换模式
	- manhattan：将任意角度的边转换为水平或竖直的边
	- diagonal ： 将任意角度的边转换为45°的斜边

### Set [[Marks]] Step

### Corner Chop Command

- pu.chop_corner: 可以切除Manhattan [[polygon]]的转角处切除一个正方形或直角三角形
```python
general_setting = {}
special_setting = []
special_rule = pu.EdgeSelection()
special_rule.add_selection({‘length':[0, 80]})
special_rule.anchor_special_setting({'chop_length': 10, 'chop_mode': 'triangle'})
special_setting.append(special_rule)
layer_chop = pu.chop_corner(layer_main, general_setting, special_setting)
```
- pu.chop_acute 可以切除[[polygon]]中包含45°的锐角部分，且在切除后原来位置变为135°.
```python
layer_chop = pu.chop_acute(layer_main, 20)
```