# what-user-agent
A bash script to humanize user-agent strings using the whatismybrowser.com API. 

Turn garbage like `Mozilla/5.0 (iPhone; CPU iPhone OS 15_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.1 Mobile/15E148 Safari/604.1` into **Safari 15.1 on iOS 15.1**


Use it like this:
```
$ what-user-agent "Mozilla/5.0 (iPhone; CPU iPhone OS 15_1 like Mac OS X) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/15.1 Mobile/15E148 Safari/604.1"
Safari 15.1 on iOS 15.1
```

Get your free API key at https://developers.whatismybrowser.com/api/signup/basic

Caches lookups so you don't use all your API calls in a month. Clear the cache by rm-ing the `$USER_AGENTS` file, which defaults to `~/.user_agents`
