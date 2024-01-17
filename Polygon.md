# [[Polygon]] Shapes Definition: 
1. SQUARE 正方形 
2. RECTANGLE 矩形 
3. MANHATTAN 除矩形和正方形外其他由水平和竖直边组成的多边形 
4. DIAGONAL 包含45°角的边且不包含非45°边的多边形
5. OTHERS 边的选择中为OTHER
# Polygon 的选择
1. 利用Polygon‘s properties例如：
    - shape 类型
    - vertex_count 点的个数
    - long_[[edge]] short_[[edge]] 长/短边的长度
    - aspect_ration 长短边之比
    - area 面积大小
    - oriantation 方向
    - [[marks]] 标签
2. 利用选择区域和Polygon位置关系进行选择
    - inside/outside 在选择区域的内外部
    - overlap 与选择区域有重合
    - interact = overlap or outside_collinear
    - intersect = overlap - inside 即有重合但是不在区域内部
    - strict_inside/strict_outside 严格在内外部无交点
    - inside_collinear/outside_collinear 内外部有重合边
    - inside_point_touch/outside_point_touch 内外部有重合点