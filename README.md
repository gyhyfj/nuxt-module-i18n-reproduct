Hi there👋

This is a minimal reproduction of [#2055](https://github.com/nuxt-modules/i18n/issues/2055)

I build a monorepo, and create two apps:
one of them is a minimal nuxt3 app,
another is a minimal csr vite-vue3 app with it's own `vue-i18n` dep.

I'm certainly sure that `vue-i18n` dep in csr-spa leads to this issue, but I must keep that dep for that app in my real project.

And nuxt3 must be used with `shamefully-hoist=true`, so I don't know how to resolve this problem in monorepo.
