# Changelog

All notable changes to this project will be documented in this file.

## [0.10.0](https://github.com/justinthelaw/uds-k3d/compare/v0.9.4...v0.10.0) (2024-10-08)


### Features

* expose gpus automagically ([#13](https://github.com/justinthelaw/uds-k3d/issues/13)) ([edaaeac](https://github.com/justinthelaw/uds-k3d/commit/edaaeace5ca498d21dfc7f4caa4ba5b6c62f4838))

## [0.9.4](https://github.com/justinthelaw/uds-k3d/compare/v0.9.3...v0.9.4) (2024-10-08)


### Bug Fixes

* defaultRuntime and publishing workflow ([#11](https://github.com/justinthelaw/uds-k3d/issues/11)) ([844fbd2](https://github.com/justinthelaw/uds-k3d/commit/844fbd23bf85f86b6a4fd3cce60340fada2cd1d0))

## [0.9.3](https://github.com/justinthelaw/uds-k3d/compare/v0.9.2...v0.9.3) (2024-10-08)


### Bug Fixes

* gpu docs and wsl issues ([#10](https://github.com/justinthelaw/uds-k3d/issues/10)) ([c3a25ca](https://github.com/justinthelaw/uds-k3d/commit/c3a25ca1a7cd7af94f3c3034bb8c95e0efa01dfc))


### Miscellaneous

* release 0.9.3 ([9c53bbf](https://github.com/justinthelaw/uds-k3d/commit/9c53bbf9c08b1146db941fa3171d2d1ed60db9a4))

## [0.9.2](https://github.com/justinthelaw/uds-k3d/compare/v0.9.1...v0.9.2) (2024-10-08)


### Bug Fixes

* tag and release workflow ([#5](https://github.com/justinthelaw/uds-k3d/issues/5)) ([c26e575](https://github.com/justinthelaw/uds-k3d/commit/c26e5750144cae7ac78f16607655afbe0f12bf32))
* tag with write-all ([#6](https://github.com/justinthelaw/uds-k3d/issues/6)) ([5e2c763](https://github.com/justinthelaw/uds-k3d/commit/5e2c7636ac10f06a421b8a9b37133e41916dbaf9))

## [0.9.1](https://github.com/justinthelaw/uds-k3d/compare/v0.9.0...v0.9.1) (2024-10-08)


### Bug Fixes

* publishing workflows ([#3](https://github.com/justinthelaw/uds-k3d/issues/3)) ([350b6f1](https://github.com/justinthelaw/uds-k3d/commit/350b6f149141300302a9e44c0c6612565d94ae0e))

## [0.9.0](https://github.com/justinthelaw/uds-k3d/compare/v0.9.0...v0.9.0) (2024-10-08)


### ⚠ BREAKING CHANGES

* add extra port support ([#103](https://github.com/justinthelaw/uds-k3d/issues/103))

### Features

* add custom k3s image ([#55](https://github.com/justinthelaw/uds-k3d/issues/55)) ([707f7d5](https://github.com/justinthelaw/uds-k3d/commit/707f7d5b07d9ecf7317439704a3d738b42ff01fb))
* add extra port support ([#103](https://github.com/justinthelaw/uds-k3d/issues/103)) ([9299bc5](https://github.com/justinthelaw/uds-k3d/commit/9299bc5bf4da40ffd6e30596d01e5a8b50793217))
* add k3s cuda image and cuda workload capabilities ([#1](https://github.com/justinthelaw/uds-k3d/issues/1)) ([627891d](https://github.com/justinthelaw/uds-k3d/commit/627891dbbeb36b60befda1215bf65765e23898f0))
* add loki user and bucket ([#41](https://github.com/justinthelaw/uds-k3d/issues/41)) ([509114d](https://github.com/justinthelaw/uds-k3d/commit/509114d9f2269d141a1dff3b3f37ab9f8fe9e3a4))
* add minio and local-path-rwx to dev stack and refactor dev stack manifests into helm chart ([#10](https://github.com/justinthelaw/uds-k3d/issues/10)) ([3648fa0](https://github.com/justinthelaw/uds-k3d/commit/3648fa0c219f40b07a2d8ce7ebebe0afe9c22cd2))
* deploy to common 🦄 shorthand repo ([579f0b8](https://github.com/justinthelaw/uds-k3d/commit/579f0b8fb4f0aa93f03763d1e5f56e7fe4cd842c))
* implement graceful, modifiable CoreDNS helm overrides ([#112](https://github.com/justinthelaw/uds-k3d/issues/112)) ([7fe1876](https://github.com/justinthelaw/uds-k3d/commit/7fe1876859af840e47ff1acc03b93733748cd4f9))
* initial release ([f66ef5f](https://github.com/justinthelaw/uds-k3d/commit/f66ef5f5283c31c7bd3ca48610775f032a4f9af1))
* internal uds.dev resolution ([#46](https://github.com/justinthelaw/uds-k3d/issues/46)) ([e677483](https://github.com/justinthelaw/uds-k3d/commit/e67748334ec45ab3a4361eaea9d674d0d9d4a5c8))
* publish multi/arm/amd packages for UDS CLI happiness ([#6](https://github.com/justinthelaw/uds-k3d/issues/6)) ([861ce6d](https://github.com/justinthelaw/uds-k3d/commit/861ce6d4c76edc283b8737929f7a071aecce1fb3))
* rewrite answer as well ([#51](https://github.com/justinthelaw/uds-k3d/issues/51)) ([baf69f6](https://github.com/justinthelaw/uds-k3d/commit/baf69f6ceb89d03eec6c1fc68783d72cb4e5ad85))
* switch to nginx from haproxy for lower resource use ([#35](https://github.com/justinthelaw/uds-k3d/issues/35)) ([041226f](https://github.com/justinthelaw/uds-k3d/commit/041226f59f5bb151679fc0070d81d52357ffcaf4))
* use daemonset for machineid instead of docker mount ([#8](https://github.com/justinthelaw/uds-k3d/issues/8)) ([2a49404](https://github.com/justinthelaw/uds-k3d/commit/2a494044e71228a29cdb102d3f85e53dd4873f35))
* use uds-dev-stack for all namespaces ([#23](https://github.com/justinthelaw/uds-k3d/issues/23)) ([3e80c89](https://github.com/justinthelaw/uds-k3d/commit/3e80c890d4649f0f48675a266b306dff68934c40))


### Bug Fixes

* add k3d to test workflow ([ae46119](https://github.com/justinthelaw/uds-k3d/commit/ae461191641f7151259fa48deea88fee3dfae70d))
* add zarf var for k3d_extra_args ([#32](https://github.com/justinthelaw/uds-k3d/issues/32)) ([6f8cb93](https://github.com/justinthelaw/uds-k3d/commit/6f8cb93cf8d568e12fdf1e217c11905249b730e4))
* broken validate task ([#71](https://github.com/justinthelaw/uds-k3d/issues/71)) ([fbe6146](https://github.com/justinthelaw/uds-k3d/commit/fbe6146536d93f2ebcb89a67176df72bbd44f198))
* buildx for publish image ([#59](https://github.com/justinthelaw/uds-k3d/issues/59)) ([427af5c](https://github.com/justinthelaw/uds-k3d/commit/427af5c615d1b8f9f87a68dab97d13ad483e99c3))
* package release workflow ([efa0d22](https://github.com/justinthelaw/uds-k3d/commit/efa0d228b4345c6c4cd9170cd35a43c43fa7c7dd))
* update policy value and document using minio ([#26](https://github.com/justinthelaw/uds-k3d/issues/26)) ([b564248](https://github.com/justinthelaw/uds-k3d/commit/b564248e739ee016085d7ae101d0cb7dd6955b75))
* update release process for zarf 0.32 ([#36](https://github.com/justinthelaw/uds-k3d/issues/36)) ([a8a9acb](https://github.com/justinthelaw/uds-k3d/commit/a8a9acb28098ae4aa0e7b3c783e86b4f567995b4))


### Miscellaneous

* add codeowners ([87f67ea](https://github.com/justinthelaw/uds-k3d/commit/87f67ead297ed78634ba65fd9fcab1d6a7a9dfd5))
* allow volumeexpansion in localpath storageclass ([#111](https://github.com/justinthelaw/uds-k3d/issues/111)) ([4d0fb5c](https://github.com/justinthelaw/uds-k3d/commit/4d0fb5cae7c7ab0a0f971a4df07e5ab36ec90516))
* **deps:** pin dependencies ([#66](https://github.com/justinthelaw/uds-k3d/issues/66)) ([122380a](https://github.com/justinthelaw/uds-k3d/commit/122380afe200f251eac85f51df1de06cbf082337))
* **deps:** replace docker image k8s.gcr.io/pause to 3.9 ([#13](https://github.com/justinthelaw/uds-k3d/issues/13)) ([0235f05](https://github.com/justinthelaw/uds-k3d/commit/0235f050bd355e21372c90e3f1cd914b0e0479f3))
* **deps:** update actions/checkout digest to 692973e ([#84](https://github.com/justinthelaw/uds-k3d/issues/84)) ([ff44cce](https://github.com/justinthelaw/uds-k3d/commit/ff44cce500216ab57f17e01b97e440c9120339ad))
* **deps:** update actions/checkout digest to a5ac7e5 ([#70](https://github.com/justinthelaw/uds-k3d/issues/70)) ([01422ba](https://github.com/justinthelaw/uds-k3d/commit/01422ba11eb5b68664691953067c4baa45f03713))
* **deps:** update defenseunicorns/uds-common action to v0.2.2 ([#50](https://github.com/justinthelaw/uds-k3d/issues/50)) ([e34753d](https://github.com/justinthelaw/uds-k3d/commit/e34753d62034b711443707443a9ff8cfd4a96e97))
* **deps:** update defenseunicorns/uds-common action to v0.4.2 ([#61](https://github.com/justinthelaw/uds-k3d/issues/61)) ([c92cf9d](https://github.com/justinthelaw/uds-k3d/commit/c92cf9d4356f164dead4a58eeeca55e1e612f62d))
* **deps:** update defenseunicorns/uds-common action to v0.4.3 ([#77](https://github.com/justinthelaw/uds-k3d/issues/77)) ([4960e94](https://github.com/justinthelaw/uds-k3d/commit/4960e946159d4681c235e5303f9ecb6a69fcbac0))
* **deps:** update defenseunicorns/uds-common action to v0.8.0 ([#81](https://github.com/justinthelaw/uds-k3d/issues/81)) ([f9eab1d](https://github.com/justinthelaw/uds-k3d/commit/f9eab1dcc0c89e5d425cce1fe89bbb022964e4ba))
* **deps:** update defenseunicorns/uds-common digest to a6fba9c ([#72](https://github.com/justinthelaw/uds-k3d/issues/72)) ([d2da739](https://github.com/justinthelaw/uds-k3d/commit/d2da739759c5a973c91db0dfee39377881dddfc8))
* **deps:** update dependency defenseunicorns/zarf to v0.31.2 ([#14](https://github.com/justinthelaw/uds-k3d/issues/14)) ([3e433f4](https://github.com/justinthelaw/uds-k3d/commit/3e433f48e2269d78ed51634e580c69ca44e4401a))
* **deps:** update dependency defenseunicorns/zarf to v0.31.3 ([#20](https://github.com/justinthelaw/uds-k3d/issues/20)) ([758ad7c](https://github.com/justinthelaw/uds-k3d/commit/758ad7c57da2d5cb930ca48e5becfddd3d5054cc))
* **deps:** update dependency defenseunicorns/zarf to v0.31.4 ([#29](https://github.com/justinthelaw/uds-k3d/issues/29)) ([e32e831](https://github.com/justinthelaw/uds-k3d/commit/e32e831a2f531bc0a257063cd6c5e030d92b42be))
* **deps:** update dependency defenseunicorns/zarf to v0.32.1 ([#34](https://github.com/justinthelaw/uds-k3d/issues/34)) ([cd8db52](https://github.com/justinthelaw/uds-k3d/commit/cd8db5287113946683241b941f4006ce26222406))
* **deps:** update dependency defenseunicorns/zarf to v0.32.4 ([#39](https://github.com/justinthelaw/uds-k3d/issues/39)) ([0dd4735](https://github.com/justinthelaw/uds-k3d/commit/0dd4735f93b50cad786459747108190536e544fd))
* **deps:** update dev-stack to v0.0.29 ([#102](https://github.com/justinthelaw/uds-k3d/issues/102)) ([402b20e](https://github.com/justinthelaw/uds-k3d/commit/402b20eb32cac3f19b0bc4cbc49e9578a60dca49))
* **deps:** update docker image k8s.gcr.io/pause to v3.9 ([#17](https://github.com/justinthelaw/uds-k3d/issues/17)) ([c3b6e0c](https://github.com/justinthelaw/uds-k3d/commit/c3b6e0c29a5d77917ba38eafbdd51436bcda0f37))
* **deps:** update docker image rancher/local-path-provisioner to v0.0.26 ([#16](https://github.com/justinthelaw/uds-k3d/issues/16)) ([e8a4a63](https://github.com/justinthelaw/uds-k3d/commit/e8a4a63aa61b17a790cebe57e60d02ec9912351f))
* **deps:** update docker/login-action digest to 0d4c9c5 ([#79](https://github.com/justinthelaw/uds-k3d/issues/79)) ([0fcbb5a](https://github.com/justinthelaw/uds-k3d/commit/0fcbb5af5e6ba72fb24f718f4625aced8c7ec1d5))
* **deps:** update docker/setup-buildx-action action to v3.2.0 ([#54](https://github.com/justinthelaw/uds-k3d/issues/54)) ([e7a639d](https://github.com/justinthelaw/uds-k3d/commit/e7a639d75f1fc3b8a49f0963a1cb8e4ea7ec0cfc))
* **deps:** update docker/setup-buildx-action action to v3.3.0 ([#68](https://github.com/justinthelaw/uds-k3d/issues/68)) ([770d3ed](https://github.com/justinthelaw/uds-k3d/commit/770d3ed9e3905a4a5a9668e6a8051b081893ffe2))
* **deps:** update docker/setup-buildx-action action to v3.4.0 ([#87](https://github.com/justinthelaw/uds-k3d/issues/87)) ([85cc784](https://github.com/justinthelaw/uds-k3d/commit/85cc7843a4a90109f7782c47fd9264a6755ea66f))
* **deps:** update githubactions ([#110](https://github.com/justinthelaw/uds-k3d/issues/110)) ([868ace5](https://github.com/justinthelaw/uds-k3d/commit/868ace5468e7366f44720812cb1203b6d5a69f66))
* **deps:** update githubactions ([#94](https://github.com/justinthelaw/uds-k3d/issues/94)) ([fda8d99](https://github.com/justinthelaw/uds-k3d/commit/fda8d99ce4925822e2bbfbe2610aa928e306182d))
* **deps:** update githubactions ([#96](https://github.com/justinthelaw/uds-k3d/issues/96)) ([a730642](https://github.com/justinthelaw/uds-k3d/commit/a730642d76d2ada2695350ac360a9e3bd8d86847))
* **deps:** update githubactions to v0.12.0 ([#101](https://github.com/justinthelaw/uds-k3d/issues/101)) ([d110f93](https://github.com/justinthelaw/uds-k3d/commit/d110f937a2c07e3fc107bcf1a01f2b56ea7a3130))
* **deps:** update google-github-actions/release-please-action action to v4 ([#21](https://github.com/justinthelaw/uds-k3d/issues/21)) ([8e8400d](https://github.com/justinthelaw/uds-k3d/commit/8e8400de5a83f3702eb94a59471eb2f99cdc21df))
* **deps:** update google-github-actions/release-please-action digest to e4dc86b ([#74](https://github.com/justinthelaw/uds-k3d/issues/74)) ([27e0723](https://github.com/justinthelaw/uds-k3d/commit/27e0723c7c5a453ad8fc8c109596d1726ca96508))
* **deps:** update googleapis/release-please-action action to v4.1.3 ([#82](https://github.com/justinthelaw/uds-k3d/issues/82)) ([2ede840](https://github.com/justinthelaw/uds-k3d/commit/2ede84035b20d652541efefa1eabc50eae7c8024))
* **deps:** update helm release metallb to v0.14.5 ([#62](https://github.com/justinthelaw/uds-k3d/issues/62)) ([381ec21](https://github.com/justinthelaw/uds-k3d/commit/381ec21285f770c3186705244c1b20736286d129))
* **deps:** update helm release metallb to v0.14.6 ([#90](https://github.com/justinthelaw/uds-k3d/issues/90)) ([5c510bb](https://github.com/justinthelaw/uds-k3d/commit/5c510bbac61528096fec2dd38c2a067ece3986d3))
* **deps:** update helm release minio to v5.2.0 ([#63](https://github.com/justinthelaw/uds-k3d/issues/63)) ([d826b55](https://github.com/justinthelaw/uds-k3d/commit/d826b550d33c1df6b8899501b8d011d064f9bfa2))
* **deps:** update metallb to v0.14.8 ([#93](https://github.com/justinthelaw/uds-k3d/issues/93)) ([b9c61c6](https://github.com/justinthelaw/uds-k3d/commit/b9c61c625447ce2894a6660c6c207cf5b5258b8c))
* **deps:** update rancher/local-path-provisioner docker tag to v0.0.28 ([#80](https://github.com/justinthelaw/uds-k3d/issues/80)) ([d9af211](https://github.com/justinthelaw/uds-k3d/commit/d9af2113a061b309000ddf6b554680068b176e87))
* **deps:** update registry.k8s.io/pause docker tag to v3.10 ([#78](https://github.com/justinthelaw/uds-k3d/issues/78)) ([85b6fa4](https://github.com/justinthelaw/uds-k3d/commit/85b6fa46a7b92c925fefa84b0b16738513704d2b))
* **deps:** update uds-common to v0.13.0 ([#107](https://github.com/justinthelaw/uds-k3d/issues/107)) ([ac3f60d](https://github.com/justinthelaw/uds-k3d/commit/ac3f60d611e2edf29ca09b404cf70630768fd385))
* **docs:** graceful k3d shutdown and startup ([#100](https://github.com/justinthelaw/uds-k3d/issues/100)) ([876a19b](https://github.com/justinthelaw/uds-k3d/commit/876a19b6984d9269354d6618befc819e3adaa006))
* fix codeowners ([#97](https://github.com/justinthelaw/uds-k3d/issues/97)) ([6daf597](https://github.com/justinthelaw/uds-k3d/commit/6daf597ef0872e53c29c431a44aa45e9bbb2d663))
* fix codeowners file ([#42](https://github.com/justinthelaw/uds-k3d/issues/42)) ([a108b5f](https://github.com/justinthelaw/uds-k3d/commit/a108b5f70a43f6dba8e2bc68043e5015d721be94))
* fix readme release annotation ([d0ea198](https://github.com/justinthelaw/uds-k3d/commit/d0ea1987e3a69f06dece471eb96a51bbdf232ff2))
* **main:** release 0.1.10 ([#5](https://github.com/justinthelaw/uds-k3d/issues/5)) ([8f374b2](https://github.com/justinthelaw/uds-k3d/commit/8f374b24ab8cafb21e34eb1fbc9e6b83288e69b4))
* **main:** release 0.1.11 ([#7](https://github.com/justinthelaw/uds-k3d/issues/7)) ([d99e36c](https://github.com/justinthelaw/uds-k3d/commit/d99e36c7e401e9cba5966e905d3340782dfee0e1))
* **main:** release 0.1.12 ([#9](https://github.com/justinthelaw/uds-k3d/issues/9)) ([e50ffd6](https://github.com/justinthelaw/uds-k3d/commit/e50ffd6d06829c752887308987a8346b1bd0a5a4))
* **main:** release 0.1.13 ([#12](https://github.com/justinthelaw/uds-k3d/issues/12)) ([dfc3833](https://github.com/justinthelaw/uds-k3d/commit/dfc38331a48ee88dfab74f05b9a4fc5e766b947e))
* **main:** release 0.1.14 ([#19](https://github.com/justinthelaw/uds-k3d/issues/19)) ([8e50d0c](https://github.com/justinthelaw/uds-k3d/commit/8e50d0c5021e41496fcf679da250eaf1d2daa5f5))
* **main:** release 0.1.7 ([fd111b1](https://github.com/justinthelaw/uds-k3d/commit/fd111b146723a1fd96fca5cecd7144b7335c9ba1))
* **main:** release 0.1.8 ([#3](https://github.com/justinthelaw/uds-k3d/issues/3)) ([92f8e30](https://github.com/justinthelaw/uds-k3d/commit/92f8e301e95e0b4fed3ff9ae2f4970ba546489c7))
* **main:** release 0.1.9 ([#4](https://github.com/justinthelaw/uds-k3d/issues/4)) ([4c04225](https://github.com/justinthelaw/uds-k3d/commit/4c04225ff1df9b9121eafd266a78a281700e115f))
* **main:** release 0.2.0 ([#22](https://github.com/justinthelaw/uds-k3d/issues/22)) ([fa52092](https://github.com/justinthelaw/uds-k3d/commit/fa520929159988f3d3008d983b2aac53ced03589))
* **main:** release 0.2.1 ([#27](https://github.com/justinthelaw/uds-k3d/issues/27)) ([ed75072](https://github.com/justinthelaw/uds-k3d/commit/ed75072975006539cb094309b73bbaf7e2c8362c))
* **main:** release 0.3.0 ([#33](https://github.com/justinthelaw/uds-k3d/issues/33)) ([2e1514f](https://github.com/justinthelaw/uds-k3d/commit/2e1514f05338be57d29071ef31aad3fa2ef92a65))
* **main:** release 0.3.1 ([#38](https://github.com/justinthelaw/uds-k3d/issues/38)) ([01ed1fe](https://github.com/justinthelaw/uds-k3d/commit/01ed1fee82c4d00a612f779802bc5c624630b9ef))
* **main:** release 0.4.0 ([#43](https://github.com/justinthelaw/uds-k3d/issues/43)) ([c7cc6fa](https://github.com/justinthelaw/uds-k3d/commit/c7cc6fae8c814bafc92566a6a553029401d8ce8b))
* **main:** release 0.5.0 ([#44](https://github.com/justinthelaw/uds-k3d/issues/44)) ([b36ab06](https://github.com/justinthelaw/uds-k3d/commit/b36ab069b7363d73e38b1198715e98b3928d4d2e))
* **main:** release 0.6.0 ([#52](https://github.com/justinthelaw/uds-k3d/issues/52)) ([487f2e4](https://github.com/justinthelaw/uds-k3d/commit/487f2e48b6580444e3e6f3014ad3bbb6396e48dd))
* **main:** release 0.7.0 ([#57](https://github.com/justinthelaw/uds-k3d/issues/57)) ([bec028e](https://github.com/justinthelaw/uds-k3d/commit/bec028e4077c1f531ef26db5424a30d5253653d7))
* **main:** release 0.8.0 ([#91](https://github.com/justinthelaw/uds-k3d/issues/91)) ([fd71acd](https://github.com/justinthelaw/uds-k3d/commit/fd71acdc94d7fc3ebc1812352ae085062649c2f1))
* **main:** release 0.9.0 ([#95](https://github.com/justinthelaw/uds-k3d/issues/95)) ([53dbe09](https://github.com/justinthelaw/uds-k3d/commit/53dbe09d6d386854e3e53b962f47910a6ace62e8))
* make release-please less stupid ([#18](https://github.com/justinthelaw/uds-k3d/issues/18)) ([01b36ae](https://github.com/justinthelaw/uds-k3d/commit/01b36aecb35ffd5433647f2dffe82bb59bf676d1))
* release config work ([c3523dc](https://github.com/justinthelaw/uds-k3d/commit/c3523dc9d3e2ad74f308b3c786c021a51c6fb29f))
* switch to common renovate config ([#60](https://github.com/justinthelaw/uds-k3d/issues/60)) ([61e015b](https://github.com/justinthelaw/uds-k3d/commit/61e015bcb37d811ec0f7cec0c3762d7650190064))
* update codeowners ([#69](https://github.com/justinthelaw/uds-k3d/issues/69)) ([9f6391d](https://github.com/justinthelaw/uds-k3d/commit/9f6391d955430e5fb6587f26e63adfc28a15cd59))
* update k3s test versions, default to 1.30.4 ([#104](https://github.com/justinthelaw/uds-k3d/issues/104)) ([1aa5cb3](https://github.com/justinthelaw/uds-k3d/commit/1aa5cb3489e0df6e9115dad1b11baffb55ca7409))
* update k3s version, comment out custom image (https://github.com/defenseunicorns/uds-k3d/pull/92) ([9a5776d](https://github.com/justinthelaw/uds-k3d/commit/9a5776d824cffe75078b3af6abd43de7dabcb2c1))
* update renovate config ([#11](https://github.com/justinthelaw/uds-k3d/issues/11)) ([d3a44bc](https://github.com/justinthelaw/uds-k3d/commit/d3a44bcbd043357b8fbbb5794a771d3452b3f286))
* update to latest k3s patches, switch port mapping to standard ports ([#76](https://github.com/justinthelaw/uds-k3d/issues/76)) ([6339460](https://github.com/justinthelaw/uds-k3d/commit/63394606f77a8c78c7b47b8c46a7d8a6b88c1157))

## [0.9.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.8.0...v0.9.0) (2024-09-17)


### ⚠ BREAKING CHANGES

* add extra port support ([#103](https://github.com/defenseunicorns/uds-k3d/issues/103))

### Features

* add extra port support ([#103](https://github.com/defenseunicorns/uds-k3d/issues/103)) ([9299bc5](https://github.com/defenseunicorns/uds-k3d/commit/9299bc5bf4da40ffd6e30596d01e5a8b50793217))


### Miscellaneous

* **deps:** update dev-stack to v0.0.29 ([#102](https://github.com/defenseunicorns/uds-k3d/issues/102)) ([402b20e](https://github.com/defenseunicorns/uds-k3d/commit/402b20eb32cac3f19b0bc4cbc49e9578a60dca49))
* **deps:** update githubactions ([#94](https://github.com/defenseunicorns/uds-k3d/issues/94)) ([fda8d99](https://github.com/defenseunicorns/uds-k3d/commit/fda8d99ce4925822e2bbfbe2610aa928e306182d))
* **deps:** update githubactions ([#96](https://github.com/defenseunicorns/uds-k3d/issues/96)) ([a730642](https://github.com/defenseunicorns/uds-k3d/commit/a730642d76d2ada2695350ac360a9e3bd8d86847))
* **deps:** update githubactions to v0.12.0 ([#101](https://github.com/defenseunicorns/uds-k3d/issues/101)) ([d110f93](https://github.com/defenseunicorns/uds-k3d/commit/d110f937a2c07e3fc107bcf1a01f2b56ea7a3130))
* **deps:** update metallb to v0.14.8 ([#93](https://github.com/defenseunicorns/uds-k3d/issues/93)) ([b9c61c6](https://github.com/defenseunicorns/uds-k3d/commit/b9c61c625447ce2894a6660c6c207cf5b5258b8c))
* **docs:** graceful k3d shutdown and startup ([#100](https://github.com/defenseunicorns/uds-k3d/issues/100)) ([876a19b](https://github.com/defenseunicorns/uds-k3d/commit/876a19b6984d9269354d6618befc819e3adaa006))
* fix codeowners ([#97](https://github.com/defenseunicorns/uds-k3d/issues/97)) ([6daf597](https://github.com/defenseunicorns/uds-k3d/commit/6daf597ef0872e53c29c431a44aa45e9bbb2d663))
* update k3s test versions, default to 1.30.4 ([#104](https://github.com/defenseunicorns/uds-k3d/issues/104)) ([1aa5cb3](https://github.com/defenseunicorns/uds-k3d/commit/1aa5cb3489e0df6e9115dad1b11baffb55ca7409))

## [0.8.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.7.0...v0.8.0) (2024-07-16)


### Miscellaneous

* **deps:** update actions/checkout digest to 692973e ([#84](https://github.com/defenseunicorns/uds-k3d/issues/84)) ([ff44cce](https://github.com/defenseunicorns/uds-k3d/commit/ff44cce500216ab57f17e01b97e440c9120339ad))
* **deps:** update defenseunicorns/uds-common action to v0.8.0 ([#81](https://github.com/defenseunicorns/uds-k3d/issues/81)) ([f9eab1d](https://github.com/defenseunicorns/uds-k3d/commit/f9eab1dcc0c89e5d425cce1fe89bbb022964e4ba))
* **deps:** update docker/login-action digest to 0d4c9c5 ([#79](https://github.com/defenseunicorns/uds-k3d/issues/79)) ([0fcbb5a](https://github.com/defenseunicorns/uds-k3d/commit/0fcbb5af5e6ba72fb24f718f4625aced8c7ec1d5))
* **deps:** update docker/setup-buildx-action action to v3.4.0 ([#87](https://github.com/defenseunicorns/uds-k3d/issues/87)) ([85cc784](https://github.com/defenseunicorns/uds-k3d/commit/85cc7843a4a90109f7782c47fd9264a6755ea66f))
* **deps:** update googleapis/release-please-action action to v4.1.3 ([#82](https://github.com/defenseunicorns/uds-k3d/issues/82)) ([2ede840](https://github.com/defenseunicorns/uds-k3d/commit/2ede84035b20d652541efefa1eabc50eae7c8024))
* **deps:** update helm release metallb to v0.14.6 ([#90](https://github.com/defenseunicorns/uds-k3d/issues/90)) ([5c510bb](https://github.com/defenseunicorns/uds-k3d/commit/5c510bbac61528096fec2dd38c2a067ece3986d3))
* **deps:** update rancher/local-path-provisioner docker tag to v0.0.28 ([#80](https://github.com/defenseunicorns/uds-k3d/issues/80)) ([d9af211](https://github.com/defenseunicorns/uds-k3d/commit/d9af2113a061b309000ddf6b554680068b176e87))
* **deps:** update registry.k8s.io/pause docker tag to v3.10 ([#78](https://github.com/defenseunicorns/uds-k3d/issues/78)) ([85b6fa4](https://github.com/defenseunicorns/uds-k3d/commit/85b6fa46a7b92c925fefa84b0b16738513704d2b))
* update k3s version, comment out custom image (https://github.com/defenseunicorns/uds-k3d/pull/92) ([9a5776d](https://github.com/defenseunicorns/uds-k3d/commit/9a5776d824cffe75078b3af6abd43de7dabcb2c1))

## [0.7.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.6.0...v0.7.0) (2024-05-23)


### Features

* add custom k3s image ([#55](https://github.com/defenseunicorns/uds-k3d/issues/55)) ([707f7d5](https://github.com/defenseunicorns/uds-k3d/commit/707f7d5b07d9ecf7317439704a3d738b42ff01fb))


### Bug Fixes

* broken validate task ([#71](https://github.com/defenseunicorns/uds-k3d/issues/71)) ([fbe6146](https://github.com/defenseunicorns/uds-k3d/commit/fbe6146536d93f2ebcb89a67176df72bbd44f198))
* buildx for publish image ([#59](https://github.com/defenseunicorns/uds-k3d/issues/59)) ([427af5c](https://github.com/defenseunicorns/uds-k3d/commit/427af5c615d1b8f9f87a68dab97d13ad483e99c3))


### Miscellaneous

* **deps:** pin dependencies ([#66](https://github.com/defenseunicorns/uds-k3d/issues/66)) ([122380a](https://github.com/defenseunicorns/uds-k3d/commit/122380afe200f251eac85f51df1de06cbf082337))
* **deps:** update actions/checkout digest to a5ac7e5 ([#70](https://github.com/defenseunicorns/uds-k3d/issues/70)) ([01422ba](https://github.com/defenseunicorns/uds-k3d/commit/01422ba11eb5b68664691953067c4baa45f03713))
* **deps:** update defenseunicorns/uds-common action to v0.4.2 ([#61](https://github.com/defenseunicorns/uds-k3d/issues/61)) ([c92cf9d](https://github.com/defenseunicorns/uds-k3d/commit/c92cf9d4356f164dead4a58eeeca55e1e612f62d))
* **deps:** update defenseunicorns/uds-common action to v0.4.3 ([#77](https://github.com/defenseunicorns/uds-k3d/issues/77)) ([4960e94](https://github.com/defenseunicorns/uds-k3d/commit/4960e946159d4681c235e5303f9ecb6a69fcbac0))
* **deps:** update defenseunicorns/uds-common digest to a6fba9c ([#72](https://github.com/defenseunicorns/uds-k3d/issues/72)) ([d2da739](https://github.com/defenseunicorns/uds-k3d/commit/d2da739759c5a973c91db0dfee39377881dddfc8))
* **deps:** update docker/setup-buildx-action action to v3.2.0 ([#54](https://github.com/defenseunicorns/uds-k3d/issues/54)) ([e7a639d](https://github.com/defenseunicorns/uds-k3d/commit/e7a639d75f1fc3b8a49f0963a1cb8e4ea7ec0cfc))
* **deps:** update docker/setup-buildx-action action to v3.3.0 ([#68](https://github.com/defenseunicorns/uds-k3d/issues/68)) ([770d3ed](https://github.com/defenseunicorns/uds-k3d/commit/770d3ed9e3905a4a5a9668e6a8051b081893ffe2))
* **deps:** update google-github-actions/release-please-action action to v4 ([#21](https://github.com/defenseunicorns/uds-k3d/issues/21)) ([8e8400d](https://github.com/defenseunicorns/uds-k3d/commit/8e8400de5a83f3702eb94a59471eb2f99cdc21df))
* **deps:** update google-github-actions/release-please-action digest to e4dc86b ([#74](https://github.com/defenseunicorns/uds-k3d/issues/74)) ([27e0723](https://github.com/defenseunicorns/uds-k3d/commit/27e0723c7c5a453ad8fc8c109596d1726ca96508))
* **deps:** update helm release metallb to v0.14.5 ([#62](https://github.com/defenseunicorns/uds-k3d/issues/62)) ([381ec21](https://github.com/defenseunicorns/uds-k3d/commit/381ec21285f770c3186705244c1b20736286d129))
* **deps:** update helm release minio to v5.2.0 ([#63](https://github.com/defenseunicorns/uds-k3d/issues/63)) ([d826b55](https://github.com/defenseunicorns/uds-k3d/commit/d826b550d33c1df6b8899501b8d011d064f9bfa2))
* switch to common renovate config ([#60](https://github.com/defenseunicorns/uds-k3d/issues/60)) ([61e015b](https://github.com/defenseunicorns/uds-k3d/commit/61e015bcb37d811ec0f7cec0c3762d7650190064))
* update codeowners ([#69](https://github.com/defenseunicorns/uds-k3d/issues/69)) ([9f6391d](https://github.com/defenseunicorns/uds-k3d/commit/9f6391d955430e5fb6587f26e63adfc28a15cd59))
* update to latest k3s patches, switch port mapping to standard ports ([#76](https://github.com/defenseunicorns/uds-k3d/issues/76)) ([6339460](https://github.com/defenseunicorns/uds-k3d/commit/63394606f77a8c78c7b47b8c46a7d8a6b88c1157))

## [0.6.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.5.0...v0.6.0) (2024-03-09)


### Features

* rewrite answer as well ([#51](https://github.com/defenseunicorns/uds-k3d/issues/51)) ([baf69f6](https://github.com/defenseunicorns/uds-k3d/commit/baf69f6ceb89d03eec6c1fc68783d72cb4e5ad85))


### Miscellaneous

* **deps:** update defenseunicorns/uds-common action to v0.2.2 ([#50](https://github.com/defenseunicorns/uds-k3d/issues/50)) ([e34753d](https://github.com/defenseunicorns/uds-k3d/commit/e34753d62034b711443707443a9ff8cfd4a96e97))

## [0.5.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.4.0...v0.5.0) (2024-03-01)


### Features

* internal uds.dev resolution ([#46](https://github.com/defenseunicorns/uds-k3d/issues/46)) ([e677483](https://github.com/defenseunicorns/uds-k3d/commit/e67748334ec45ab3a4361eaea9d674d0d9d4a5c8))


### Miscellaneous

* **deps:** update dependency defenseunicorns/zarf to v0.32.4 ([#39](https://github.com/defenseunicorns/uds-k3d/issues/39)) ([0dd4735](https://github.com/defenseunicorns/uds-k3d/commit/0dd4735f93b50cad786459747108190536e544fd))
* fix codeowners file ([#42](https://github.com/defenseunicorns/uds-k3d/issues/42)) ([a108b5f](https://github.com/defenseunicorns/uds-k3d/commit/a108b5f70a43f6dba8e2bc68043e5015d721be94))

## [0.4.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.3.1...v0.4.0) (2024-02-16)


### Features

* add loki user and bucket ([#41](https://github.com/defenseunicorns/uds-k3d/issues/41)) ([509114d](https://github.com/defenseunicorns/uds-k3d/commit/509114d9f2269d141a1dff3b3f37ab9f8fe9e3a4))

## [0.3.1](https://github.com/defenseunicorns/uds-k3d/compare/v0.3.0...v0.3.1) (2024-01-17)


### Bug Fixes

* add zarf var for k3d_extra_args ([#32](https://github.com/defenseunicorns/uds-k3d/issues/32)) ([6f8cb93](https://github.com/defenseunicorns/uds-k3d/commit/6f8cb93cf8d568e12fdf1e217c11905249b730e4))

## [0.3.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.2.1...v0.3.0) (2024-01-10)


### Features

* switch to nginx from haproxy for lower resource use ([#35](https://github.com/defenseunicorns/uds-k3d/issues/35)) ([041226f](https://github.com/defenseunicorns/uds-k3d/commit/041226f59f5bb151679fc0070d81d52357ffcaf4))


### Bug Fixes

* update release process for zarf 0.32 ([#36](https://github.com/defenseunicorns/uds-k3d/issues/36)) ([a8a9acb](https://github.com/defenseunicorns/uds-k3d/commit/a8a9acb28098ae4aa0e7b3c783e86b4f567995b4))


### Miscellaneous

* **deps:** update dependency defenseunicorns/zarf to v0.31.4 ([#29](https://github.com/defenseunicorns/uds-k3d/issues/29)) ([e32e831](https://github.com/defenseunicorns/uds-k3d/commit/e32e831a2f531bc0a257063cd6c5e030d92b42be))
* **deps:** update dependency defenseunicorns/zarf to v0.32.1 ([#34](https://github.com/defenseunicorns/uds-k3d/issues/34)) ([cd8db52](https://github.com/defenseunicorns/uds-k3d/commit/cd8db5287113946683241b941f4006ce26222406))

## [0.2.1](https://github.com/defenseunicorns/uds-k3d/compare/v0.2.0...v0.2.1) (2023-12-07)


### Bug Fixes

* update policy value and document using minio ([#26](https://github.com/defenseunicorns/uds-k3d/issues/26)) ([b564248](https://github.com/defenseunicorns/uds-k3d/commit/b564248e739ee016085d7ae101d0cb7dd6955b75))

## [0.2.0](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.14...v0.2.0) (2023-12-04)


### Features

* use uds-dev-stack for all namespaces ([#23](https://github.com/defenseunicorns/uds-k3d/issues/23)) ([3e80c89](https://github.com/defenseunicorns/uds-k3d/commit/3e80c890d4649f0f48675a266b306dff68934c40))


### Miscellaneous

* **deps:** update docker image rancher/local-path-provisioner to v0.0.26 ([#16](https://github.com/defenseunicorns/uds-k3d/issues/16)) ([e8a4a63](https://github.com/defenseunicorns/uds-k3d/commit/e8a4a63aa61b17a790cebe57e60d02ec9912351f))

## [0.1.14](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.13...v0.1.14) (2023-11-30)


### Miscellaneous

* **deps:** update dependency defenseunicorns/zarf to v0.31.3 ([#20](https://github.com/defenseunicorns/uds-k3d/issues/20)) ([758ad7c](https://github.com/defenseunicorns/uds-k3d/commit/758ad7c57da2d5cb930ca48e5becfddd3d5054cc))
* make release-please less stupid ([#18](https://github.com/defenseunicorns/uds-k3d/issues/18)) ([01b36ae](https://github.com/defenseunicorns/uds-k3d/commit/01b36aecb35ffd5433647f2dffe82bb59bf676d1))

## [0.1.13](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.12...v0.1.13) (2023-11-29)


### Features

* add minio and local-path-rwx to dev stack and refactor dev stack manifests into helm chart ([#10](https://github.com/defenseunicorns/uds-k3d/issues/10)) ([3648fa0](https://github.com/defenseunicorns/uds-k3d/commit/3648fa0c219f40b07a2d8ce7ebebe0afe9c22cd2))


### Miscellaneous

* **deps:** replace docker image k8s.gcr.io/pause to 3.9 ([#13](https://github.com/defenseunicorns/uds-k3d/issues/13)) ([0235f05](https://github.com/defenseunicorns/uds-k3d/commit/0235f050bd355e21372c90e3f1cd914b0e0479f3))
* **deps:** update dependency defenseunicorns/zarf to v0.31.2 ([#14](https://github.com/defenseunicorns/uds-k3d/issues/14)) ([3e433f4](https://github.com/defenseunicorns/uds-k3d/commit/3e433f48e2269d78ed51634e580c69ca44e4401a))
* **deps:** update docker image k8s.gcr.io/pause to v3.9 ([#17](https://github.com/defenseunicorns/uds-k3d/issues/17)) ([c3b6e0c](https://github.com/defenseunicorns/uds-k3d/commit/c3b6e0c29a5d77917ba38eafbdd51436bcda0f37))
* update renovate config ([#11](https://github.com/defenseunicorns/uds-k3d/issues/11)) ([d3a44bc](https://github.com/defenseunicorns/uds-k3d/commit/d3a44bcbd043357b8fbbb5794a771d3452b3f286))

## [0.1.12](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.11...v0.1.12) (2023-11-09)


### Features

* use daemonset for machineid instead of docker mount ([#8](https://github.com/defenseunicorns/uds-k3d/issues/8)) ([2a49404](https://github.com/defenseunicorns/uds-k3d/commit/2a494044e71228a29cdb102d3f85e53dd4873f35))

## [0.1.11](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.10...v0.1.11) (2023-11-02)


### Features

* publish multi/arm/amd packages for UDS CLI happiness ([#6](https://github.com/defenseunicorns/uds-k3d/issues/6)) ([861ce6d](https://github.com/defenseunicorns/uds-k3d/commit/861ce6d4c76edc283b8737929f7a071aecce1fb3))

## [0.1.10](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.9...v0.1.10) (2023-10-30)


### Bug Fixes

* add k3d to test workflow ([ae46119](https://github.com/defenseunicorns/uds-k3d/commit/ae461191641f7151259fa48deea88fee3dfae70d))


### Miscellaneous

* add codeowners ([87f67ea](https://github.com/defenseunicorns/uds-k3d/commit/87f67ead297ed78634ba65fd9fcab1d6a7a9dfd5))

## [0.1.9](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.8...v0.1.9) (2023-10-30)


### Features

* deploy to common 🦄 shorthand repo ([579f0b8](https://github.com/defenseunicorns/uds-k3d/commit/579f0b8fb4f0aa93f03763d1e5f56e7fe4cd842c))


### Miscellaneous

* fix readme release annotation ([d0ea198](https://github.com/defenseunicorns/uds-k3d/commit/d0ea1987e3a69f06dece471eb96a51bbdf232ff2))

## [0.1.8](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.7...v0.1.8) (2023-10-30)


### Bug Fixes

* package release workflow ([efa0d22](https://github.com/defenseunicorns/uds-k3d/commit/efa0d228b4345c6c4cd9170cd35a43c43fa7c7dd))

## [0.1.7](https://github.com/defenseunicorns/uds-k3d/compare/v0.1.6...v0.1.7) (2023-10-30)


### Features

* initial release ([f66ef5f](https://github.com/defenseunicorns/uds-k3d/commit/f66ef5f5283c31c7bd3ca48610775f032a4f9af1))


### Miscellaneous

* release config work ([c3523dc](https://github.com/defenseunicorns/uds-k3d/commit/c3523dc9d3e2ad74f308b3c786c021a51c6fb29f))

## [0.0.0] - YYYY-MM-DD
PRE RELEASE

### Added
- Initial CHANGELOG.md
- CODEOWNERS
- CONTRIBUTING.md
- DEVELOPMENT_MAINTENANCE.md
- LICENSE
- READEME.md
- zarf.yaml
