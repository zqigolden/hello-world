overlap 范围 | 是否采用 | 类别
-------- | ----- | ------
overlaps >= cfg.TRAIN.FG_THRESH | 是 | overlap最大类别
overlaps < cfg.TRAIN.BG_THRESH_HI and overlaps >= cfg.TRAIN.BG_THRESH_LO | 是 | background
overlaps < cfg.TRAIN.BG_THRESH_LO | 否 | None
