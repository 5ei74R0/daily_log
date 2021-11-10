# 2021/11/8 (MON)

<div class="date_jumper">
  <a class="link_wrapper" href="./7th.md"><div class="button">go to the previous day</div></a>
  <a class="link_wrapper" href="./9th.md"><div class="button">go to the next day</div></a>
</div>

## Univ.
- visited a lab.

### courses
#### *Experiment*
- Intelligent Robotics

### homework
#### *Experiment*
- report

## Memo, Feelings, Thoughts
- IoU (Intersection over Union)
  - Note! : we treat pixels
  ```python
  class BBox:
    def __init__(self, x1: int, x2: int, y1: int, y2: int):
      """
      x in [x1, x2)
      y in [y1, y2)
      """
      self.x1 = x1
      self.x2 = x2
      self.y1 = y1
      self.y2 = y2
      self.area = (x2 - x1 + 1) * (y2 - y1 + 1)

  def calc_iou(a: BBox, b: BBox):
    x_intersection = max(0, min(a.x2, b.x2) - max(a.x1, b.x1) + 1)
    y_intersection = max(0, min(a.y2, b.y2) - max(a.y1, b.y1) + 1)
    intersection = x_intersection * y_intersection
    union = a.area + b.area - intersection
    return intersection / union
  ```
- GIoU (Generalized Intersection over Union)
  ```python
  def calc_giou(a: BBox, b: BBox):
    x_intersection = max(0, min(a.x2, b.x2) - max(a.x1, b.x1) + 1)
    y_intersection = max(0, min(a.y2, b.y2) - max(a.y1, b.y1) + 1)
    intersection = x_intersection * y_intersection
    union = a.area + b.area - intersection

    c_x = max(a.x2, b.x2) - min(a.x1, b.x1) + 1
    c_y = max(a.y2, b.y2) - min(a.y1, b.y1) + 1
    c_area = c_x * c_y
    return intersection / union - (c_area - union) / c_area
  ```
