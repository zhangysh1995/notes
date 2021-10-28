## crontab 命令
*  什么是 crontab -> [crontab(5) Linux Man Page](https://man7.org/linux/man-pages/man5/crontab.5.html)
> A crontab file contains instructions for the cron(8) daemon in
> the following simplified manner: "run this command at this time on this date".  

*  `crontab` 是用户命令，用来管理加载的定时任务
*  `cron` 是 demon，实际执行使用 crontab 添加的任务
*  `crontab` 配置文件避坑
	*  文件需要用 newline 结束，按回车在最后添加空行
	*  `$PATH` 环境变量不会加载 `/etc/profile` 或 `.bashrc` 等，需要手动指定
	*  时间格式参考 Man Page
*  定时任务不能运行，参考以下指南
	*  [How to fix all of your crontab related woes/problems (Linux)](https://serverfault.com/a/449652/428439)
