miniflux-notifier
=================

Checks your [Miniflux](https://github.com/miniflux/miniflux) instance for new
articles and dispatches a desktop notification.

## Set Up Options

Export the following environment variables:

| Variable      |
|---------------|
| MINIFLUX_URL  |
| MINIFLUX_USER |
| MINIFLUX_PASS |

Run the script!

```
./miniflux-notifier
```

Alternatively, you can export the script to a supervisor. Write your variables
to `.env`, and use [foreman](https://github.com/ddollar/foreman) or
[forego](https://github.com/ddollar/forego) to export configurations.

```
foreman export upstart ~/.config/upstart --app miniflux-notifier
```
