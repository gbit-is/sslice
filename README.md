# About
I did some research on the SSL usage of .is domains and I [wrote a blog about it](https://biomech.xyz/2018/04/03/iceland-and-https/).

I wrote the blog about a dataset I gathered from checking 17.4K .is URLs. After gathering the data for it I recieved 2 additional URL lists that increased my URL list to 53K. Out of those 53K, 27,5K didn't answer http requests and 43K didn't answer https requests.

After running the larger set I did a quick look and the statistics I gathered presented in the blog scaled-ish. so I see no need to modify the blog itself. However I had some requests to publish the raw data. Which is the purpose of this repo

# So, what do we have here ?
this repo is just a json file and this file explaining it

Example

	'https_redir': True,                                  # Does port 80 forward to 443
	'name': 'totallyarealurl.is',                         # The URL in question
	'notbefore': 'NotBefore: Mar3112: 10: 422018GMT',     # Start date of cert in a mangled format, sorry about that
	'notafter': 'NotAfter: Jun2912: 10: 422018GMT',       # End date of cert in the same mangled format
	'https_code': <Response[200]>,                        # What response code we got from https          
	'http_code': <Response[200]>,                         # What response code we got from http
	'validity': 'valid',                                  # This field seems to have failed to populate during construction of JSON
	'issuer': u"Johnies Cert Services"                    # The cert issuer, if any
