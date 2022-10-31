# DDK_Gerrit
Introduce how to install Gerrit on Linux. </br>

# What is Gerrit?
Gerrit is a kind of code collaboration (code review) tool. </br>

# Why do we need Gerrit?
We should do "code review" before updating the remote branch with local commits. </br>
It is similar to PR or MR below. </br> 
</br>
GitHub : Pull requests </br>
GitLab : Merge requests </br>

# Let us get started

## Environments
Linux ubuntu 5.13.0-30-generic #33~20.04.1-Ubuntu SMP </br>

## Download Gerrit 
Download the "gerrit-x.x.x.war" from https://gerrit-releases.storage.googleapis.com/index.html. </br>

```sh
wget https://gerrit-releases.storage.googleapis.com/gerrit-3.6.2.war
```

## Instanl Gerrit
For jdk issue, please refer to "http://blog.tonycube.com/2021/07/java-class-version.html".
```sh
sudo apt-get install openjdk-11-jdk
```

```sh
export GERRIT_SITE=~/gerrit_testsite
java -jar gerrit*.war init --batch --dev -d $GERRIT_SITE
```

... </br>

# References
1. https://gerrit-review.googlesource.com/Documentation/linux-quickstart.html
2. https://vocus.cc/article/60a48eecfd897800011a0bf0
3. https://c55jeremy-tech.blogspot.com/2019/04/gerrit-serveraosp-codebase-part-13.html
4. https://www.youtube.com/watch?v=Wxx8XndqZ7A
