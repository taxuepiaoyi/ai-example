一、申请api-key
官网地址：https://bailian.console.aliyun.com/#/home
![11](https://github.com/user-attachments/assets/6ed9c072-ad6a-47cf-a367-f59c8841509b)


二 项目中无法引入spring-ai的依赖，有可能是spring-ai的相关依赖包，还没发布到maven中央仓库，需要在pom.xml中添加以下代码：
    <repositories>
        <repository>
            <id>spring-snapshots</id>
            <url>https://repo.spring.io/snapshot</url>
            <snapshots>
                <enabled>true</enabled>
            </snapshots>
        </repository>
        <repository>
            <id>spring-milestones</id>
            <url>https://repo.spring.io/milestone</url>
        </repository>
    </repositories>
