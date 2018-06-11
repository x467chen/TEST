# TEST
Multi-thread testing

## Jmeter
1.Install [Jmeter](https://jmeter.apache.org/).<br />
2.Reach to the /bin file under Jmeter package.
3.Start Jmeter with cmd:
``` xml
 sh jmeter
```
4.Http management type:
``` xml
Content-Type
application/json
```

## Cloud
1.Go to the console to create a new instance.
2.Upload project to the new instance with cmd:
``` xml
sudo rsync -avz -e "ssh -i PathToXxx.pem" --delete --exclude=\"build\" --exclude=\"out\" --exclude=\".*/\" .  root@HostIp:~/Newfilename
```
or
``` xml
scp ~/Downloads/xxx.txt root@HostIp:~/xxx.txt

```

3.Configure Java8 environment, with following cmd:
``` xml
sudo apt-get update
sudo apt install --reinstall software-properties-common
sudo add-apt-repository ppa:webupd8team/java
sudo apt-get update

sudo apt-get install oracle-java8-installer
sudo apt install oracle-java8-set-default

```

4.If you project is based on spring boot
``` xml
./gradlew build bootRun
```
