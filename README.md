# University of Guelph IoT Project




## All Resource Links
- Github Repository: [https://github.com/The-Ahmed-Shahriar/IoT-Project](https://github.com/The-Ahmed-Shahriar/IoT-Project)
- UoGuelph Shared Docs: [uoguelphca-my.sharepoint.com](https://uoguelphca-my.sharepoint.com/:f:/r/personal/ashahr01_uoguelph_ca/Documents/UoGuelph%20IoT%20Project?csf=1&web=1&e=Kde6Pv)
- EMQX Serverless Broker: [https://www.emqx.com/en/cloud/serverless-mqtt](https://www.emqx.com/en/cloud/serverless-mqtt)
- Discord: [https://discord.gg/mmjgTt3r2J](https://discord.gg/mmjgTt3r2J)




## Summary
This code base offers a basic IoT communication pipeline to measure data with sensors remotely. You can track multiple sensors, from various remote microcontroller devices that are remotely.

Currently, this respository is on version **1.0.1**. Change log:
- Now compatablile with DHT11 sensor
- Documentation




## Prerequisites
1. Setup hardware, if applicable (e.g., a Raspberry Pi)
2. Ensure you have access to a CLI on your device - Linux recommended
3. Check if you have git installed with the `$ git --version` command, install if needed
4. Install Golang ([Official](https://go.dev/doc/install)), ([Recommended Tutorial](https://www.jeremymorgan.com/tutorials/raspberry-pi/install-go-raspberry-pi/)); check with `$ go version`
5. Setup EMQX broker ([EMQX Docs](https://uoguelphca-my.sharepoint.com/:b:/r/personal/ashahr01_uoguelph_ca/Documents/UoGuelph%20IoT%20Project/Onboarding/EMQX%20Broker%20Setup%20and%20Testing.pdf?csf=1&web=1&e=y4eJ1y))




## Installation and Execution
First, clone this repository:
```
$ git clone https://github.com/The-Ahmed-Shahriar/IoT-Project.git
```

Once cloned, traverse to the `./EMQX/defs.go` file and insert your broker information to the following constants (see [EMQX Docs](https://uoguelphca-my.sharepoint.com/:b:/r/personal/ashahr01_uoguelph_ca/Documents/UoGuelph%20IoT%20Project/Onboarding/EMQX%20Broker%20Setup%20and%20Testing.pdf?csf=1&web=1&e=y4eJ1y) for where to find these parameters).
```
 7  const (
 8  	BROKER_HOST = ""
 9  	CLIENT_ID   = ""
10  	CLIENT_USER = ""
11  	CLIENT_PSWD = ""
12  )
```

Ensure that your EMQX broker instance is running. Then, run your cloned repository as a Go program:
```
$ go run <path_to_directory>
```

For example, when in the cloned directory's root:
```
$ go run .
```




## Licence
[MIT License](LICENSE)
