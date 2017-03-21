# 服务器安装gitlab

1.什么是gitlab
    * gitlab 是一个 git 项目托管仓库
    * gitlab 是开源的
    * gitlab 是免费的
    * gitlab 可以被私人搭建使用

2.gitlab 官方网站
    http://www.gitlab.com

3.ubuntu 16.04 安装　gitlab 
    参考资料：https://mirrors.tuna.tsinghua.edu.cn/help/gitlab-ce/
    安装步骤：
        1.首先信任 GitLab 的 GPG 公钥:
           curl https://packages.gitlab.com/gpg.key 2> /dev/null | sudo apt-key add - &>/dev/null
        2.给ubuntu系统添加第三方源
            sudo vi /etc/apt/sources.list.d/gitlab-ce.list
            在上述打开文件中，添加下一行
            deb https://mirrors.tuna.tsinghua.edu.cn/gitlab-ce/ubuntu xenial main
        3.更新源
            sudo apt-get update
        4.安装gitlab
            sudo apt-get install gitlab-ce

4.ubuntu 16.04 安装　gitlab 
    参考资料：https://mirrors.tuna.tsinghua.edu.cn/help/gitlab-ci-multi-runner/
        安装步骤：
            1.首先信任 GitLab 的 GPG 公钥:
            curl https://packages.gitlab.com/gpg.key 2> /dev/null | sudo apt-key add - &>/dev/null
            2.给ubuntu系统添加第三方源
                sudo vi /etc/apt/sources.list.d/gitlab-ci-multi-runner.list
                在上述打开文件中，添加下一行
                deb https://mirrors.tuna.tsinghua.edu.cn/gitlab-ci-multi-runner/ubuntu xenial main
            3.更新源
                sudo apt-get update
            4.安装gitlab
                sudo apt-get install gitlab-ci-multi-runner