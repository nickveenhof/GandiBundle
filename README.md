# EDSI-Tech Gandi Bundle

Gandi API v3


## Install

1. Install the bundle with composer

`composer require edsi-tech/gandi-bundle: dev-master`

2. Register the Bundle

Add in your AppKernel.php  `new EdsiTech\GandiBundle\EdsiTechGandiBundle(),`

3. Add the mandatory configurations options

In your app/config/config.yml

```yaml
 edsitech_gandi:
    server_url: "https://rpc.ote.gandi.net/xmlrpc/"
    api_key: 
    default_nameservers:
        - dns1.edsi-tech.com
        - dns2.edsi-tech.com
        - dns3.edsi-tech.com
    default_handles:
        bill: XYZ-GANDI
        tech: XYZ-GANDI
        admin: XYZ-GANDI
        owner: XYZ-GANDI
        
```

Note that the test server is `https://rpc.ote.gandi.net/xmlrpc/` and the production server is `https://rpc.gandi.net/xmlrpc/`

## Testing

Launch `vendor/phpunit/phpunit/phpunit Tests/`
