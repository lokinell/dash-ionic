# Ionic docset generator for dash

Prerequisites: ruby, bundler

Generation:

1. ```git clone https://github.com/DarkSwoop/dash-ionic.git```
2. ```cd dash-ionic```
3. ```bundle install```
4. ```rake```

The docset will be created in the ```dist``` folder. 

# Problem
1. libxml2 cannot find
```
	brew install libxml2
	bundle config build.nokogiri "--use-system-libraries --with-xml2-include=/usr/local/opt/libxml2/include/libxml2" 
	bundle install
```


2. run rake 碰到 「ArgumentError: invalid byte sequence in US-ASCII」

```
➜  dash-ionic git:(master) ✗ export LANGUAGE=en.US.UTF-8
➜  dash-ionic git:(master) ✗ export LANG=en_US.UTF-8
➜  dash-ionic git:(master) ✗ export LANGUAGE=en_US.UTF-8
➜  dash-ionic git:(master) ✗ export LC_ALL=en_US.UTF-8
```

