# DevOpsToolsChainDeploy
1.jenkins官方最新镜像
docker pull jenkins/jenkins;
docker save -o jenkins.tar jenkins/jenkins;
2.nexus3官方最新镜像
docker pull sonatype/nexus3
docker save -o nexus3.tar sonatype/nexus3;
3.并复制jenkins.tar、nexus3.tar文件到site.yml同级目录；
4.执行playbook安装：ansible-playbook -i hosts -e @vars site.yml
