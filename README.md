⚠️ *DEPRECATED* ⚠️ This connector is now built in to [opsdroid core](https://opsdroid.readthedocs.io/en/stable/connectors/facebook/). This repository only exists for backward compatibility and will be removed.

# opsdroid connector facebook

A connector for [opsdroid](https://github.com/opsdroid/opsdroid) to interact with Facebook messenger.

## Usage

**This connector requires that the opsdroid web server is internet facing.**

 - Create a Facbook page for your bot
 - Visit https://developers.facebook.com
 - Create a new app and add a messenger product
 - Generate a `page-access-token` for the page you created
 - Create a webhook pointing to `http(s)://your-bot-url.com:port/connector/facebook`
 - Randomly generate a `verify-token` and add that to the webhook

## Configuration

```yaml
connectors:
  - name: facebook
    # required
    verify-token: aabbccddee
    page-access-token: aabbccddee112233445566
    # optional
    bot-name: "mybot" # default "opsdroid"
```
