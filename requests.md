# Requests: HTTP for humans

Requests is a HTTP library for Python. Requests allows you to send organic HTTP requests, without the need for manual labor.

You can use Requests module to communicate with 3rd-party APIs.

[Requests documentation](http://docs.python-requests.org/en/latest/index.html)

## Sample

```
>>> import requests
>>> r = requests.get('https://api.github.com/user', auth=('user', 'pass'))
>>> r.status_code
200
>>> r.headers['content-type']
'application/json; charset=utf8'
>>> r.encoding
'utf-8'
>>> r.text
u'{"type":"User"...'
>>> r.json()
{u'private_gists': 419, u'total_private_repos': 77, ...}
```
## Include Requests module

```
import requests
```

## HTTP commands for the Internet transfer control

|HTTP Command | Description|
|-------------|------------|
|GET | Retrieves the document from the specified URL|
|HEAD | Gets the head information|
|POST | Sends data to the server |
|PUT| Replaces the page with the specified URL with the specified data|

## Send requests

```
>>> r = requests.get('https://api.github.com/events')
>>> r = requests.post('http://httpbin.org/post', data = {'key':'value'})
>>> r = requests.put('http://httpbin.org/put', data = {'key':'value'})
>>> r = requests.delete('http://httpbin.org/delete')
>>> r = requests.head('http://httpbin.org/get')
>>> r = requests.options('http://httpbin.org/get')
```
