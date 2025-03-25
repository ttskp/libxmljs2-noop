# @ttskp/libxmljs2-noop

[libxmljs2](https://www.npmjs.com/package/libxmljs2) has critical, unresolved security issues, ([CVE-2024-34393](https://github.com/advisories/GHSA-mjr4-7xg5-pfvh), [CVE-2024-34394](https://github.com/advisories/GHSA-78h3-pg4x-j8cv)), but is no longer maintained. libxmljs2-noop is a "no-op" package without any implementation. It can be used to replace libxmljs2 to silence security alerts in projects where libxmljs2 is included by npm as an optional, transitive dependency, but not actually used.

To replace libxmljs2 with @ttskp/libxmljs2-noop, decleare the following `override` in your `package.json`:

```json
{
    "overrides": {
        "libxmljs2": "https://registry.npmjs.org/@ttskp/libxmljs2-noop/-/libxmljs2-noop-1.0.0.tgz"
    }
}
```
