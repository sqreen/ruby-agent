# Sqreen agent for Ruby

## Support

Need assistance? You can create an issue here, but shoot an email to `support@sqreen.com` for a timely response.

We encourage you to go through the [compatibility](https://docs.sqreen.com/ruby/compatibility/) and [troubleshooting](https://docs.sqreen.com/ruby/troubleshooting/) pages first.

## Documentation

See https://docs.sqreen.com.

See also https://blog.sqreen.com/dynamic-instrumentation-agent-for-ruby/ for a "behind-the-scenes" post.

## Viewing the agent code

The agent code is not open source, but you can audit the agent code from the gem itself in your favourite editor:

```
bundle show sqreen  # (deprecated) gives path to the active and installed sqreen gem
bundle info sqreen  # gives info, including path to the active and installed sqreen gem
bundle edit sqreen  # opens sqreen gem directory with $EDITOR
```

Alternatively, fetch and decompress the gem manually:

```bash
gem="sqreen"
version="1.23.0"
curl -O "https://rubygems.org/downloads/${gem}-${version}.gem"
mkdir "${gem}-${version}"
tar -C "${gem}-${version}" -xf "${gem}-${version}".gem
tar -C "${gem}-${version}" -xzf "${gem}-${version}"/data.tar.gz
"${EDITOR:-vim}" "${gem}-${version}"
```
