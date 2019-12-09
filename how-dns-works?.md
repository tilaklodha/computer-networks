How DNS works?

The communication over internet happens with IP addresses. All the human readable web addresses are linked with a IP address. Whenver you type "www.google.com" in browser following things will happen:

- The browser and OS layer will check whether they have any corresponding ip addreess related to www.google.com.
- Then comes the resolver which is in most cases is our internet service provider. The resolver first looks into it's own cache or otherwise knows where all the root servers are located.
- The root server knows where the top level domain server is for `.com`
- The `.com` server will give the authorative nameservers for `www.google.com`
- Once we know about the ANS then it's just one final step knowing the final ip of `www.google.com`
- Resolver takes that ip and goes back to os layer and browser and both of them caches the ip for further queries.

Reference: [How dns works](https://howdns.works/)

