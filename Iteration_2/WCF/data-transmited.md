---
title: Data Transmited
parent: WCF Service
grand_parent: Iteration 2
has_children: false
---

## Data Transmited

Example of **App.config** configuration:
```
<?xml version="1.0" encoding="utf-8" ?>
<configuration>
    <startup> 
        <supportedRuntime version="v4.0" sku=".NETFramework,Version=v4.6.1" />
    </startup>
  <system.serviceModel>
    <services>
      <service name="Host.ChatService">
        <endpoint address=""
                  binding="wsDualHttpBinding"
                  contract="Host.IChatService">
        </endpoint>
        <host>
          <baseAddresses>
            <add baseAddress="http://localhost:9090"/>
          </baseAddresses>
        </host>
      </service>
    </services>
    <behaviors>
      <serviceBehaviors>
        <behavior>
          <serviceMetadata httpGetEnabled="true"/>
        </behavior>
      </serviceBehaviors>
    </behaviors>
  </system.serviceModel>
</configuration>
```

![Localhost](../../images/final-assignment/Localhost.PNG)