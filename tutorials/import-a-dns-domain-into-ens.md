# Import a DNS domain into ENS

### Introduction

DNSSEC (The Domain Name System Security Extensions) establishes a chain of trust from the root key which signed by ICANN (.) and down through each key. Given DNSSEC is enabled and an ETH address is put into the subdomain of the domain you own (eg: `_ens.yourdomain.tld`), ENS manager allows anyone to submit the hash of the chain to `DNSSEC Oracle` smart contract

### Step 1

When you first land on ENS manager, you will see something like below.

![](../.gitbook/assets/linkens1.png)

If your DNS provider already supports DNSSEC-signed domains, all you do is to enable the option on the DNS manager. If they don’t, you’ll need to migrate to someone who does.

We recommend either [EasyDNS](https://www.easydns.com) or [Google Cloud DNS](https://cloudplatform.googleblog.com/2017/11/DNSSEC-now-available-in-Cloud-DNS.html). EasyDNS’s setup guide for DNSSEC is [here](https://fusion.easydns.com/Knowledgebase/Article/View/18/7/dnssec), while Google’s is [here](https://cloud.google.com/dns/dnssec-config). Whatever provider you need, make sure you select RSA signatures and SHA256 hashing to not incur the high gas fees of trying to link your ENS name with ECDSA keys.

#### A list of popular hosting providers and which key types they support for their DNSSEC configuration

* **Native ENS integration**
  * [easyDNS](https://easydns.com/)
* **RSA/SHA-256 / ECDSA**
  * [Google Cloud DNS](https://cloud.google.com/dns)
  * [Bluehost](https://www.bluehost.com/)
  * [Hostinger](https://hostinger.com)
  * [Hostgator](https://hostgator.com)
* **ECDSA only**
  * [GoDaddy](https://www.godaddy.com)
*   **No DNSSEC support**

    * [Wordpress](https://www.wordpress.com) _when used as the DNS provider._

    __

    __

![](../.gitbook/assets/linkens2.png)

### Step 2: Adding a TXT-record

The DNS Registrar on ENS looks for a TXT record with a specific name and format in order to verify what Ethereum address should be given ownership of the domain. To claim ownership of [mydomain.xyz](https://mydomain.xyz), create a TXT record in your DNS zone, \_[ens.mydomain.xyz](https://ens.mydomain.xyz), with text data of the form a=0x1234... where 0x1234... is the Ethereum address you want to give control of the ENS record to.

![](../.gitbook/assets/linkens3.png)

### Step 3: Registering the name into ENS

Once you get to this stage, you can complete the rest from ENS manager. Simply press "Register" and send the transaction.

![](../.gitbook/assets/linkens4.png)

### Step 4: Go to the manager

![](../.gitbook/assets/linkens5.png)
