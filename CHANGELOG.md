# [1.7.0](https://github.com/databk/rustdesk-console/compare/1.6.0...1.7.0) (2026-07-22)


### Bug Fixes

* **auth:** align login API with RustDesk client requirements ([#214](https://github.com/databk/rustdesk-console/issues/214)) ([3c2ae52](https://github.com/databk/rustdesk-console/commit/3c2ae52644dce52fe242b19b64ca3a2f7c782d30))
* **auth:** prevent TFA secret exposure in login flow ([#221](https://github.com/databk/rustdesk-console/issues/221)) ([e3a7b0a](https://github.com/databk/rustdesk-console/commit/e3a7b0a998638712265aaca7bcdd96bbb2f17880))
* **auth:** use server-generated secret for login flow control instead of user-controlled tfaCode ([#230](https://github.com/databk/rustdesk-console/issues/230)) ([dfa9250](https://github.com/databk/rustdesk-console/commit/dfa9250053f3d3016ee94b648fb19e263b8e7746))
* disable unsafe type rules for test files in eslint config ([#226](https://github.com/databk/rustdesk-console/issues/226)) ([cd19d1e](https://github.com/databk/rustdesk-console/commit/cd19d1eea12d2dd3e8001ad8caaff4ce16113f83))
* **sysinfo:** return SYSINFO_UPDATED and ID_NOT_FOUND responses ([#222](https://github.com/databk/rustdesk-console/issues/222)) ([3468e97](https://github.com/databk/rustdesk-console/commit/3468e972e7a531eb57d2120f72cded97af23756d))


### Features

* **ab:** support adding IP devices to address book ([#213](https://github.com/databk/rustdesk-console/issues/213)) ([2ba9295](https://github.com/databk/rustdesk-console/commit/2ba9295d9d9e699646ca69ff81e634b0de017699)), closes [#196](https://github.com/databk/rustdesk-console/issues/196)
* add console settings and system metrics ([#227](https://github.com/databk/rustdesk-console/issues/227)) ([45fed76](https://github.com/databk/rustdesk-console/commit/45fed7634518255ca9b1cdf7acc36343c410dc85))
* implement user groups and group-based address-book access ([#211](https://github.com/databk/rustdesk-console/issues/211)) ([1c9753c](https://github.com/databk/rustdesk-console/commit/1c9753c20f61de06f93035041160cc5201a4cce4))
* **oidc:** add PATCH sort endpoint for provider ordering ([#229](https://github.com/databk/rustdesk-console/issues/229)) ([9ca9cbb](https://github.com/databk/rustdesk-console/commit/9ca9cbb38abcccf558f42bc675eb7ced81ced746))
* separate private custom and shared address books ([#212](https://github.com/databk/rustdesk-console/issues/212)) ([0425d7f](https://github.com/databk/rustdesk-console/commit/0425d7fa4c2487567e0269cf0dfcfdbb8d81f147))
* upgrade to Node.js 24, add ARM64 Docker build, and SEA support ([#210](https://github.com/databk/rustdesk-console/issues/210)) ([5b6eb96](https://github.com/databk/rustdesk-console/commit/5b6eb96d8ce699ce24634ec1bc27ae938f6e5365))
* **user:** adapt display_name field in user APIs ([#215](https://github.com/databk/rustdesk-console/issues/215)) ([7daf01b](https://github.com/databk/rustdesk-console/commit/7daf01b2243bc3a04580c220254ed9dee12ab3cd))
* **user:** add user group update to updateUser API ([#224](https://github.com/databk/rustdesk-console/issues/224)) ([1aecf6b](https://github.com/databk/rustdesk-console/commit/1aecf6bd2d5428f7df8e09ccb1dd23d367fd5ed2))
* **user:** implement complete invite user flow ([#223](https://github.com/databk/rustdesk-console/issues/223)) ([0a966e4](https://github.com/databk/rustdesk-console/commit/0a966e466b04b4090e51d95385bb4194c6ffb3f4))



# [1.6.0](https://github.com/databk/rustdesk-console/compare/1.5.1...1.6.0) (2026-07-15)


### Bug Fixes

* make SMTP username and password fields optional ([#194](https://github.com/databk/rustdesk-console/issues/194)) ([eae647c](https://github.com/databk/rustdesk-console/commit/eae647c464ddc08019c4f7063e7cd425ec7503c1)), closes [#193](https://github.com/databk/rustdesk-console/issues/193)
* **update-check:** fix update check API URL and package.json path issues ([#207](https://github.com/databk/rustdesk-console/issues/207)) ([1d1bc6e](https://github.com/databk/rustdesk-console/commit/1d1bc6e92ec881c88d2c32ab129dba81cf686fad))


### Features

* add nexus module for custom client generation ([#192](https://github.com/databk/rustdesk-console/issues/192)) ([a8c0fcf](https://github.com/databk/rustdesk-console/commit/a8c0fcfede80ee2d5a591e283361540ddfa1edb3))
* add update check module ([#182](https://github.com/databk/rustdesk-console/issues/182)) ([b952d41](https://github.com/databk/rustdesk-console/commit/b952d414071635675c328ce22cbbb1cf4e8ed64a))



## [1.5.1](https://github.com/databk/rustdesk-console/compare/1.5.0...1.5.1) (2026-06-26)


### Bug Fixes

* map os field to standardized platform constants in /ab/peers response ([#178](https://github.com/databk/rustdesk-console/issues/178)) ([c1b0d67](https://github.com/databk/rustdesk-console/commit/c1b0d676717d7d93631d9d0358380d63d328775d)), closes [#175](https://github.com/databk/rustdesk-console/issues/175)
* merge saved LDAP config when testing connection ([#180](https://github.com/databk/rustdesk-console/issues/180)) ([7390ca5](https://github.com/databk/rustdesk-console/commit/7390ca54a364c7f91933239ac72aeed6b68774d8))
* specify varchar type for User.email column ([#181](https://github.com/databk/rustdesk-console/issues/181)) ([924bcda](https://github.com/databk/rustdesk-console/commit/924bcdaf6834b7face280e931db0070878767069))
* store null instead of empty string for user email to avoid unique constraint violation ([#176](https://github.com/databk/rustdesk-console/issues/176)) ([cff06b7](https://github.com/databk/rustdesk-console/commit/cff06b77fbf009eab533730935f542ee8bc83395)), closes [#173](https://github.com/databk/rustdesk-console/issues/173)



# [1.5.0](https://github.com/databk/rustdesk-console/compare/1.4.1...1.5.0) (2026-06-14)


### Bug Fixes

* align alarm audit query interface with file/connection audit ([#138](https://github.com/databk/rustdesk-console/issues/138)) ([825af6a](https://github.com/databk/rustdesk-console/commit/825af6a4dddb4fc02d1f37353d616dfb90072a99))


### Features

* add audit log auto-cleanup with configurable retention ([#143](https://github.com/databk/rustdesk-console/issues/143)) ([e83545a](https://github.com/databk/rustdesk-console/commit/e83545a0e13f4c097a2d24ba52a4b3a4fc52a143))
* add LDAP authentication support ([#148](https://github.com/databk/rustdesk-console/issues/148)) ([efa90ec](https://github.com/databk/rustdesk-console/commit/efa90ecbf3766c7825f1a2f2a0f0d91814afb410)), closes [#135](https://github.com/databk/rustdesk-console/issues/135)



## [1.4.1](https://github.com/databk/rustdesk-console/compare/1.4.0...1.4.1) (2026-06-07)


### Bug Fixes

* **docker:** use login-options endpoint for health check ([#133](https://github.com/databk/rustdesk-console/issues/133)) ([aab6d92](https://github.com/databk/rustdesk-console/commit/aab6d92a687c1ccdf0581b1a502601e9abdb3557))



