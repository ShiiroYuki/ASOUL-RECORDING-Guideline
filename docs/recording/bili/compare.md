# 两种录播项目的比较

!!! info "另请注意：时效性"

    这个表格的内容最后一次更新在 2022/04/28，可能不再具有时效性。
    
    编辑将尝试持续更新。

|                             | [录播姬](/recording/bili/luboji) | [blrec](/recording/bili/blrec) | 备注                                                         |
| --------------------------- | -------------------------------- | ------------------------------ | ------------------------------------------------------------ |
| 部署难度                    | 低                               | 较高                           | 在 Windows 环境下，录播姬的环境配置相对比较简单。            |
| 断流及碎片修正              | ×                                | √                              | blrec 的几乎无缝录播能且只能解决主播侧或直播线路投送时的断流，似乎对录制侧的问题无能为力。 |
| 基础录制（弹幕、高清流）    | √                                | √                              | blrec 对于抵抗流主机的断开能力较强。                         |
| 自动切割（分时、分大小）    | √                                | √                              | blrec 存在分割精度低、无法自定时间的现象。                   |
| 对于收费/限定直播的录制能力 | ？                               | √                              | 如有付费直播，需要设置购买了直播门票的账号 Cookies。 详细操作请参阅本文档的附录。 |
| 推送消息                    | ？                               | √                              | 尽管录播姬提供了 WebHook 能力，但上手难度大，需要自行对接服务； blrec 内建 ServerChan 和 PushPlus 两个推送服务，也内建发送邮件推送和WebHook能力。 |
| 网页面板                    | ×                                | √                              | 录播姬开发者说 ”计划添加“ ~~没发就是咕咕~~ 在此建议使用 VPS 或本地无头主机的用户暂时使用 blrec 项目。 |
| 跨系统能力                  | √                                | √                              | 其中 blrec 在 *nix 环境下需要正确配置 Python 录播机在定稿之时尚未出现网页面板，亦无 GUI。不适合 Linux/Unix 用户。 |