# Changelog

## [1.53.0](https://github.com/AndrewM-F/code-foundry/compare/v1.54.1...v1.53.0) (2026-11-16)


### ⚠ BREAKING CHANGES

* automation now reads CODE_FOUNDRY_TOKEN only. Repos still carrying just RELEASE_PLEASE_TOKEN fall back to the short-lived workflow token (manual merges) until they set CODE_FOUNDRY_TOKEN.

### Features

* add a merged-lane billing orchestrator for minute-billed consumers ([#731](https://github.com/AndrewM-F/code-foundry/issues/731)) ([c10ea36](https://github.com/AndrewM-F/code-foundry/commit/c10ea360c131168fe7a8a15b5e957e7951e90b92))
* add ci eval tier with shared report contract and budget gate ([#576](https://github.com/AndrewM-F/code-foundry/issues/576)) ([c9f1826](https://github.com/AndrewM-F/code-foundry/commit/c9f182660fe433dd035a6b6ce67e2f29749b0010))
* add opt-in Vite+ task runner support ([#763](https://github.com/AndrewM-F/code-foundry/issues/763)) ([cdff3b6](https://github.com/AndrewM-F/code-foundry/commit/cdff3b623a63ee1e86c4d9bf34786cd7eb64ea62))
* add tiered validation workflow ([#301](https://github.com/AndrewM-F/code-foundry/issues/301)) ([33c74b4](https://github.com/AndrewM-F/code-foundry/commit/33c74b41d2ef59f87e6796323f46ccfcb7ef4c9d))
* **agents:** add explicit merge-workflow guidance ([68b1a71](https://github.com/AndrewM-F/code-foundry/commit/68b1a710fb20ee99cf0bb8ad553781df2c0ce4d1))
* billing-paused-dependabot ([#651](https://github.com/AndrewM-F/code-foundry/issues/651)) ([206dd61](https://github.com/AndrewM-F/code-foundry/commit/206dd61f11daec74e3d59ce34b6b863041fec45e))
* **billing:** run fast-lane executes concurrently ([#738](https://github.com/AndrewM-F/code-foundry/issues/738)) ([9d68449](https://github.com/AndrewM-F/code-foundry/commit/9d68449a33ef2d2f45805429ecde711be5a28db3))
* **ci:** add opt-in merge-group audit validation ([#549](https://github.com/AndrewM-F/code-foundry/issues/549)) ([27ea69e](https://github.com/AndrewM-F/code-foundry/commit/27ea69edd2f8de344d03bb79d443ee0792f01bd8))
* **ci:** add reversible billing pause ([#402](https://github.com/AndrewM-F/code-foundry/issues/402)) ([150e589](https://github.com/AndrewM-F/code-foundry/commit/150e589d1c0b09a5ac41f21df6453b5f04ecb94b))
* **ci:** add shared performance validation ([#492](https://github.com/AndrewM-F/code-foundry/issues/492)) ([07db18c](https://github.com/AndrewM-F/code-foundry/commit/07db18ca274990a23b92e3c881a8faacfebb2f7c))
* **ci:** enforce draft pull request readiness ([#530](https://github.com/AndrewM-F/code-foundry/issues/530)) ([baf964a](https://github.com/AndrewM-F/code-foundry/commit/baf964adf63d28c6490197daae2524ba33615d46))
* **ci:** surface ungated scheduled workflows in the billing pause controls ([#681](https://github.com/AndrewM-F/code-foundry/issues/681)) ([b7ca5ba](https://github.com/AndrewM-F/code-foundry/commit/b7ca5ba7a008eba4758067fc768b4575d037bfda))
* **cli:** add shared validation plans and agent check evidence ([#538](https://github.com/AndrewM-F/code-foundry/issues/538)) ([a5a7267](https://github.com/AndrewM-F/code-foundry/commit/a5a7267276abe07e00790bef56159e7151e02a7a))
* **cloudflare-deploy:** accept optional TURBO_TOKEN secret for remote-cached deploy builds ([#640](https://github.com/AndrewM-F/code-foundry/issues/640)) ([ece084a](https://github.com/AndrewM-F/code-foundry/commit/ece084ac7e8fe89a3a65ba64e55eba06ba7f3a98))
* **cloudflare-deploy:** cache the Bun package cache across deploy jobs ([#636](https://github.com/AndrewM-F/code-foundry/issues/636)) ([a986924](https://github.com/AndrewM-F/code-foundry/commit/a9869247f5b97520cd5874383422d292485a0c87))
* **cloudflare:** add a cf deploy mode to cloudflare-deploy.yml ([#658](https://github.com/AndrewM-F/code-foundry/issues/658)) ([86fbd02](https://github.com/AndrewM-F/code-foundry/commit/86fbd02f82e4e9c2285c71142b53f877f6058956))
* **cloudflare:** verify candidates before protected version promotion ([#535](https://github.com/AndrewM-F/code-foundry/issues/535)) ([004215b](https://github.com/AndrewM-F/code-foundry/commit/004215b6c5f47d1a4d147ef530a98a5a41612779))
* code-foundry 0.38.3 — direct workflow default, muse spark model, opencode_security_model override ([4aff75a](https://github.com/AndrewM-F/code-foundry/commit/4aff75a01b1f7bc922ec877bae4ee1c5ce0afe93))
* document Adea UI workspace receipt reuse ([#811](https://github.com/AndrewM-F/code-foundry/issues/811)) ([dc132a6](https://github.com/AndrewM-F/code-foundry/commit/dc132a673ed96438f19a099f1ee0c4ab01406f88))
* eliminate skipped checks with unified matrices and an in-gate release check ([#465](https://github.com/AndrewM-F/code-foundry/issues/465)) ([26c1f88](https://github.com/AndrewM-F/code-foundry/commit/26c1f885a461befe91160e0a4bf515fb9c0da23a))
* **eval:** run the eval tier as a managed Validation / Eval lane ([#580](https://github.com/AndrewM-F/code-foundry/issues/580)) ([c4b99bb](https://github.com/AndrewM-F/code-foundry/commit/c4b99bbf1dfd18760d36113756b88444d74a49e1))
* **fleet:** add declared inventory and resumable canary rollouts ([#536](https://github.com/AndrewM-F/code-foundry/issues/536)) ([af31454](https://github.com/AndrewM-F/code-foundry/commit/af314547135cf9a75b9d91668359573d6772743f))
* **fleet:** gate upgrades on verified release qualification ([#548](https://github.com/AndrewM-F/code-foundry/issues/548)) ([7347463](https://github.com/AndrewM-F/code-foundry/commit/73474634da8ab40b6d8b30c3578fa3d922987fce))
* fold the Turbo impact check into the cloudflare deploy job ([#655](https://github.com/AndrewM-F/code-foundry/issues/655)) ([a31be90](https://github.com/AndrewM-F/code-foundry/commit/a31be90cb3e3df2b4d51f9e074329c5878b7f542))
* fold the Turbo impact check into the delivery candidate job ([#676](https://github.com/AndrewM-F/code-foundry/issues/676)) ([15db132](https://github.com/AndrewM-F/code-foundry/commit/15db1328a0e3f59d12fd7e879103ca45e02fc7c4))
* forward TURBO_API to validation and cloudflare deploy builds ([#638](https://github.com/AndrewM-F/code-foundry/issues/638)) ([4f6386f](https://github.com/AndrewM-F/code-foundry/commit/4f6386f79851c6f099d9ccac842d38825d592bd2))
* make staging-release opt-in and direct-to-main the default ([#370](https://github.com/AndrewM-F/code-foundry/issues/370)) ([da8b11a](https://github.com/AndrewM-F/code-foundry/commit/da8b11a2ed23a64d7a575df37931170bb20a37fb))
* migrate the JavaScript toolchain from ESLint/Prettier to oxlint/oxfmt ([#471](https://github.com/AndrewM-F/code-foundry/issues/471)) ([9c24004](https://github.com/AndrewM-F/code-foundry/commit/9c240041136147fa710743fe02ce81ad8060ed72))
* **node:** support Node 24 and 26, drop 20 and 22 ([#589](https://github.com/AndrewM-F/code-foundry/issues/589)) ([d5746e1](https://github.com/AndrewM-F/code-foundry/commit/d5746e113b46f2209741523ffe7a7707f0f4e4da))
* opt-in lane path filters, sccache, and nextest for Rust CI ([#626](https://github.com/AndrewM-F/code-foundry/issues/626)) ([d55379c](https://github.com/AndrewM-F/code-foundry/commit/d55379c3cd3cd03af2d097cc5af05713f76cb3d8))
* **performance:** enforce source budgets ([#499](https://github.com/AndrewM-F/code-foundry/issues/499)) ([9032631](https://github.com/AndrewM-F/code-foundry/commit/9032631fb3dae87aebc6a818a192490eb372905d))
* **performance:** standardize package audit contracts ([#501](https://github.com/AndrewM-F/code-foundry/issues/501)) ([eece9cd](https://github.com/AndrewM-F/code-foundry/commit/eece9cd2643f06a3cefcee2c4b472aaf39d26d8c))
* **pre-commit:** make the commit gate change-aware ([#702](https://github.com/AndrewM-F/code-foundry/issues/702)) ([11040e5](https://github.com/AndrewM-F/code-foundry/commit/11040e5f2213c2c55ee0eb1211367f738ecdd1c1))
* preserve repository-owned sections of managed policy documents ([#668](https://github.com/AndrewM-F/code-foundry/issues/668)) ([6c1621d](https://github.com/AndrewM-F/code-foundry/commit/6c1621d4de6198a4354c4b69b773da19c5e3623e)), closes [#667](https://github.com/AndrewM-F/code-foundry/issues/667)
* **qualification:** gate releases on installed consumer compatibility ([#544](https://github.com/AndrewM-F/code-foundry/issues/544)) ([cd51057](https://github.com/AndrewM-F/code-foundry/commit/cd510574e1815d871749d37865a8509847ac0839))
* **quality:** add opt-in site, app, Worker, and package acceptance profiles ([#545](https://github.com/AndrewM-F/code-foundry/issues/545)) ([b2b63a2](https://github.com/AndrewM-F/code-foundry/commit/b2b63a24cb12c5d87b382a9df87ece1cb26d329d))
* release-batching ([#700](https://github.com/AndrewM-F/code-foundry/issues/700)) ([7386531](https://github.com/AndrewM-F/code-foundry/commit/73865310e7b4dad71874285c05a69700775135ad))
* **release:** classify reconcile push failures and log sanitized details ([#307](https://github.com/AndrewM-F/code-foundry/issues/307)) ([b95bcdf](https://github.com/AndrewM-F/code-foundry/commit/b95bcdfc2816d93950907abc47c2ce34c3036546))
* **release:** configurable dev channel on top of batched releases ([#749](https://github.com/AndrewM-F/code-foundry/issues/749)) ([89f413b](https://github.com/AndrewM-F/code-foundry/commit/89f413b57aaea488311fba403f350f2059474df5)), closes [#699](https://github.com/AndrewM-F/code-foundry/issues/699)
* **release:** preserve caller publication overrides ([#795](https://github.com/AndrewM-F/code-foundry/issues/795)) ([e62a7f5](https://github.com/AndrewM-F/code-foundry/commit/e62a7f501293dc89d24714b81be5579c4ab871a6))
* **release:** qualify only when a release or a stuck draft needs it ([#591](https://github.com/AndrewM-F/code-foundry/issues/591)) ([40646d2](https://github.com/AndrewM-F/code-foundry/commit/40646d246764e70a0e8bbb4433e5f13e6c6cc55c))
* **release:** squash release merges, Cloudflare deploy workflow, tooling neutrality ([b294c4f](https://github.com/AndrewM-F/code-foundry/commit/b294c4f334e0cf7ae3eda0086ce4a1867459a463))
* **releases:** stage qualified assets and publish verified identical archives ([#547](https://github.com/AndrewM-F/code-foundry/issues/547)) ([96aebd5](https://github.com/AndrewM-F/code-foundry/commit/96aebd5a8df2da437875fa5df7e83964fa322a72))
* **release:** standardize generated PR titles ([#497](https://github.com/AndrewM-F/code-foundry/issues/497)) ([f61136e](https://github.com/AndrewM-F/code-foundry/commit/f61136e17f1a1828f1ec1f37e92ccfd6759d483f))
* **release:** support npm OIDC publishing ([#791](https://github.com/AndrewM-F/code-foundry/issues/791)) ([e2e47db](https://github.com/AndrewM-F/code-foundry/commit/e2e47db74bd27582f6916da39a3ec2fb81056d12))
* **releases:** verify immutable releases and attest selected build artifacts ([#537](https://github.com/AndrewM-F/code-foundry/issues/537)) ([4026bcc](https://github.com/AndrewM-F/code-foundry/commit/4026bccc759d90669ba2efd3971db57f05bd37c7))
* **release:** wire qualified draft staging and immutable publication ([#558](https://github.com/AndrewM-F/code-foundry/issues/558)) ([c48b110](https://github.com/AndrewM-F/code-foundry/commit/c48b11089882b20cd733ae6717083abea9e4b097))
* remove RELEASE_PLEASE_TOKEN fallback in favor of CODE_FOUNDRY_TOKEN ([a83a00e](https://github.com/AndrewM-F/code-foundry/commit/a83a00ea15774035875870e799cdd762972ddd2b))
* resolve lane diffs only for filtered lanes and accept injected paths ([#631](https://github.com/AndrewM-F/code-foundry/issues/631)) ([c5b6801](https://github.com/AndrewM-F/code-foundry/commit/c5b6801d87ab5211657b6f3efe8e598b5ec9f8f6))
* **runtime:** enforce an opt-in Build time ceiling ([#840](https://github.com/AndrewM-F/code-foundry/issues/840)) ([5f432fe](https://github.com/AndrewM-F/code-foundry/commit/5f432fe412f9ffb05cccb40ff871e0da528b843a))
* scope Cloudflare build variables to build ([#802](https://github.com/AndrewM-F/code-foundry/issues/802)) ([c7dcac7](https://github.com/AndrewM-F/code-foundry/commit/c7dcac717d4c55e8a5d8a989ab5a1dcbe669d9d8))
* scope CodeQL analysis to changed languages and Rust shards on pull requests ([#654](https://github.com/AndrewM-F/code-foundry/issues/654)) ([8125f02](https://github.com/AndrewM-F/code-foundry/commit/8125f02bd8eb44d75dbc5e09301d99da53371e64))
* scope per-language checks to detected languages via matrix ([#459](https://github.com/AndrewM-F/code-foundry/issues/459)) ([a18268f](https://github.com/AndrewM-F/code-foundry/commit/a18268f052b14dfb65d30a0d7aee35c785ac2259))
* skip the security detector entirely while OpenCode Security is disabled ([#653](https://github.com/AndrewM-F/code-foundry/issues/653)) ([385879b](https://github.com/AndrewM-F/code-foundry/commit/385879bd287363b0feaebd9e97e74f9b3933253c))
* support Apache 2.0 license sync ([814ee2c](https://github.com/AndrewM-F/code-foundry/commit/814ee2cf934a99e8b6fcd221284aa7dbb48fe9e1))
* support isolated integration test shards ([#783](https://github.com/AndrewM-F/code-foundry/issues/783)) ([b8f4770](https://github.com/AndrewM-F/code-foundry/commit/b8f477061b68f34925d6fcc4bf8b8f1e3530ddf0))
* **sync:** add dependency_updater setting to gate Dependabot and scaffold Renovate ([#692](https://github.com/AndrewM-F/code-foundry/issues/692)) ([7890dcc](https://github.com/AndrewM-F/code-foundry/commit/7890dccf31c2ce469e8aedba9881bbe0b27c0f4c))
* **sync:** oxfmt-stable config merges, gitignore preservation, and OPENCODE_SECURITY variable override ([c19f428](https://github.com/AndrewM-F/code-foundry/commit/c19f428758f8a41edf1aeb711e93c2f70b7eb3d3))
* **validation:** allow audit mode on staging PRs ([79cc3e0](https://github.com/AndrewM-F/code-foundry/commit/79cc3e0c9c7d918f1fe8ee3f72a89456e0f90312))
* **validation:** downgrade docs-only PRs to fast and gate bot pushes ([#590](https://github.com/AndrewM-F/code-foundry/issues/590)) ([6962c0c](https://github.com/AndrewM-F/code-foundry/commit/6962c0ccecb19a797a8e3b2a00300429adf63aeb))
* **validation:** enforce required capabilities, coverage, and task evidence ([#534](https://github.com/AndrewM-F/code-foundry/issues/534)) ([d213b85](https://github.com/AndrewM-F/code-foundry/commit/d213b8599d5e8325f66e672a0ab4076585df83c1))
* **validation:** run a lean release lane for Release Please pull requests ([#579](https://github.com/AndrewM-F/code-foundry/issues/579)) ([04ba644](https://github.com/AndrewM-F/code-foundry/commit/04ba6447bdd8e4215df51ca1b05ef1d14da2dbbb))
* **validation:** shard the managed E2E lane via e2e_shards ([#697](https://github.com/AndrewM-F/code-foundry/issues/697)) ([6e999f7](https://github.com/AndrewM-F/code-foundry/commit/6e999f7b0fc6c0f706ae8b72994bdd524ff63905))
* **validation:** skip default-branch CodeQL on release-please merges ([#694](https://github.com/AndrewM-F/code-foundry/issues/694)) ([b427b09](https://github.com/AndrewM-F/code-foundry/commit/b427b09ea83aa0c8c416be87729b7db86541ba50))
* **workflows:** protect draft pull requests by default ([#572](https://github.com/AndrewM-F/code-foundry/issues/572)) ([4071c58](https://github.com/AndrewM-F/code-foundry/commit/4071c5848d0401906f5c507f2a2a95ed91b9ea96))


### Bug Fixes

* allow isolated preview auth Hyperdrive build binding ([#813](https://github.com/AndrewM-F/code-foundry/issues/813)) ([c308145](https://github.com/AndrewM-F/code-foundry/commit/c308145c1c26d50c83e357fc7db39aa0bf46a296))
* **billing:** declare the runner inputs the callers always forward ([#733](https://github.com/AndrewM-F/code-foundry/issues/733)) ([2a4ec7a](https://github.com/AndrewM-F/code-foundry/commit/2a4ec7a65d8ba42df9d70dab62c3a11502975c87))
* **billing:** emit the codeql input as a YAML boolean ([#735](https://github.com/AndrewM-F/code-foundry/issues/735)) ([ad52921](https://github.com/AndrewM-F/code-foundry/commit/ad52921e361e275c38d56b0a1ef2283168e94555))
* **billing:** join fast-lane receipts in a second parallel group ([#742](https://github.com/AndrewM-F/code-foundry/issues/742)) ([e7c1f6d](https://github.com/AndrewM-F/code-foundry/commit/e7c1f6d5a94e21822bb97fbf27983964b53efa0e))
* **billing:** keep lint standalone; join fast-lane receipts in parallel ([#744](https://github.com/AndrewM-F/code-foundry/issues/744)) ([419f2c6](https://github.com/AndrewM-F/code-foundry/commit/419f2c6db4396cd2559428824669ddaf70a5e017))
* **ci:** cancel only superseded pull-request runs in managed workflows ([#710](https://github.com/AndrewM-F/code-foundry/issues/710)) ([77e57da](https://github.com/AndrewM-F/code-foundry/commit/77e57da9b2da147584dd1b9c1884def5e582ceed))
* **ci:** create promotion PRs through REST ([249b4a6](https://github.com/AndrewM-F/code-foundry/commit/249b4a6ec304d249b35d4c888856fe7b3e11540a))
* **ci:** declare the e2e shard inputs on the no-codeql orchestrator ([#714](https://github.com/AndrewM-F/code-foundry/issues/714)) ([9c9eb84](https://github.com/AndrewM-F/code-foundry/commit/9c9eb8417d03285f1a093b32a55e29197676a73b))
* **ci:** dedupe caller names and keep CodeQL Rust shards aligned ([#613](https://github.com/AndrewM-F/code-foundry/issues/613)) ([38d02c3](https://github.com/AndrewM-F/code-foundry/commit/38d02c3eaf10f2a14634ee5a50c69261b1988190))
* **ci:** fall back to github token for promotion ([b0e2606](https://github.com/AndrewM-F/code-foundry/commit/b0e26064de34e0ffc668510e15f6a0d73c06c956))
* **ci:** finalize direct fleet policy ([#513](https://github.com/AndrewM-F/code-foundry/issues/513)) ([f1c95c0](https://github.com/AndrewM-F/code-foundry/commit/f1c95c0032616cc1bc2066a14b0f2f52b1509699))
* **ci:** guard every workflow during billing pause ([#405](https://github.com/AndrewM-F/code-foundry/issues/405)) ([d460695](https://github.com/AndrewM-F/code-foundry/commit/d4606959d7134254f93fa91ce460604ef6e1be9b))
* **ci:** isolate default-branch security audits ([c959f56](https://github.com/AndrewM-F/code-foundry/commit/c959f5642f8f6f190a5d7cf84c23336194b5826f))
* **ci:** keep OpenCode detection visible ([#523](https://github.com/AndrewM-F/code-foundry/issues/523)) ([9283456](https://github.com/AndrewM-F/code-foundry/commit/9283456a35a3ef41fe7de578e1111fccc9805067))
* **ci:** key runtime concurrency by event so promotion PRs do not cancel push checks ([4e7c002](https://github.com/AndrewM-F/code-foundry/commit/4e7c00275d09c0a48d26bb852638ec127d5a8734))
* **ci:** launch wrangler under Node in the cloudflare deploy step ([#649](https://github.com/AndrewM-F/code-foundry/issues/649)) ([3c32b09](https://github.com/AndrewM-F/code-foundry/commit/3c32b09fdead9450015fcb7a8165d740f55d4a69))
* **ci:** restore protected consumer audits ([#503](https://github.com/AndrewM-F/code-foundry/issues/503)) ([39e53ed](https://github.com/AndrewM-F/code-foundry/commit/39e53ed88c471a8bc878ced29c2729d1a4a6c683))
* **ci:** retain scoped task receipts across success and failure ([#557](https://github.com/AndrewM-F/code-foundry/issues/557)) ([407838f](https://github.com/AndrewM-F/code-foundry/commit/407838f48a903d30767ef001c85e0747bce22111))
* **ci:** run CodeQL on every main push ([#797](https://github.com/AndrewM-F/code-foundry/issues/797)) ([b85d85e](https://github.com/AndrewM-F/code-foundry/commit/b85d85e69cb8cf7f456f28b0b230ee3a1d68ebdc))
* **ci:** run full validation on release PRs ([#517](https://github.com/AndrewM-F/code-foundry/issues/517)) ([53a6d55](https://github.com/AndrewM-F/code-foundry/commit/53a6d55c367e158ca7fae15a9ededaccb2fb1b03))
* **ci:** serialize billing receipt and report uploads ([#773](https://github.com/AndrewM-F/code-foundry/issues/773)) ([cec7afd](https://github.com/AndrewM-F/code-foundry/commit/cec7afd6263ad0113d42d08b4f4306c3e5e3b5a1))
* **ci:** stabilize runners and release reconciliation ([#387](https://github.com/AndrewM-F/code-foundry/issues/387)) ([bac3ea4](https://github.com/AndrewM-F/code-foundry/commit/bac3ea446c32d7ffc6b13b77a6e7728352e8dce2))
* **ci:** suppress unavailable and draft checks ([#507](https://github.com/AndrewM-F/code-foundry/issues/507)) ([cf70040](https://github.com/AndrewM-F/code-foundry/commit/cf700402cdd1e4a0dda0d6ad86084847c701eb0a))
* **cloudflare:** build a preview Build Output before cf previews deploy ([#660](https://github.com/AndrewM-F/code-foundry/issues/660)) ([1a9d59c](https://github.com/AndrewM-F/code-foundry/commit/1a9d59cc360f6b8aca2bffc8c7053ba881a1c5ba))
* **cloudflare:** build the production Build Output before the prebuilt deploy ([087e2bf](https://github.com/AndrewM-F/code-foundry/commit/087e2bfc3fb87da3e3efda5de7d0f5ffb4b5e80a))
* **cloudflare:** deploy previews from the prebuilt Preview Build Output ([#664](https://github.com/AndrewM-F/code-foundry/issues/664)) ([8881654](https://github.com/AndrewM-F/code-foundry/commit/88816540931b8681757c5d286017809117257d9e))
* **cloudflare:** preserve Bun package manager for OpenNext deploys ([#529](https://github.com/AndrewM-F/code-foundry/issues/529)) ([af8a282](https://github.com/AndrewM-F/code-foundry/commit/af8a282fa141ec582cebfefa1e2a6c662dbafefe))
* **cloudflare:** remove duplicate deployment records ([#595](https://github.com/AndrewM-F/code-foundry/issues/595)) ([1ddf004](https://github.com/AndrewM-F/code-foundry/commit/1ddf0047388c843db4b076b8183ed5f4fad447ac))
* **cloudflare:** resolve cf bins by walking up node_modules/.bin ([#662](https://github.com/AndrewM-F/code-foundry/issues/662)) ([a304f9c](https://github.com/AndrewM-F/code-foundry/commit/a304f9c6ee04585704ce1ecd1fcc85006875cdb1))
* **cloudflare:** surface the cf deploy error instead of discarding it ([bd79a67](https://github.com/AndrewM-F/code-foundry/commit/bd79a67f9f051d56fadd3dbf79f0ec1801aee918))
* **codeql:** analyze the pull request head commit ([#624](https://github.com/AndrewM-F/code-foundry/issues/624)) ([8494898](https://github.com/AndrewM-F/code-foundry/commit/849489885d2e11796311984dc23249d0e49d6358))
* **codeql:** pass the event name so pull request change detection runs ([#823](https://github.com/AndrewM-F/code-foundry/issues/823)) ([1dd16b9](https://github.com/AndrewM-F/code-foundry/commit/1dd16b99c199ec1f489c17d097e1c7f458517c17))
* complete runtime package declarations ([#838](https://github.com/AndrewM-F/code-foundry/issues/838)) ([f8b9bb3](https://github.com/AndrewM-F/code-foundry/commit/f8b9bb359e9e2384c66a63d680bac6281af84e93))
* **config:** pin the lint-bearing CI lane to a standard runner by default ([#718](https://github.com/AndrewM-F/code-foundry/issues/718)) ([ee462d3](https://github.com/AndrewM-F/code-foundry/commit/ee462d39ed003c74db28e9e5aacd883c366811f5))
* default runtime-ref inputs to the current runtime release ([#454](https://github.com/AndrewM-F/code-foundry/issues/454)) ([ceef1de](https://github.com/AndrewM-F/code-foundry/commit/ceef1dea2ef1a4f64bf9c6500f0699fb300108e3))
* **delivery:** drop impossible NUL guard that always failed the turbo impact check ([#607](https://github.com/AndrewM-F/code-foundry/issues/607)) ([62ee9c9](https://github.com/AndrewM-F/code-foundry/commit/62ee9c997329217812b58c9be8eb17427343ce90))
* **deploy:** send auto_inactive once when completing a deployment status ([#610](https://github.com/AndrewM-F/code-foundry/issues/610)) ([9dcdc54](https://github.com/AndrewM-F/code-foundry/commit/9dcdc543bf0167de317658f3b9f1f83d8409e528))
* **docs:** describe full release validation ([#519](https://github.com/AndrewM-F/code-foundry/issues/519)) ([f01e770](https://github.com/AndrewM-F/code-foundry/commit/f01e77015e37e2436d4729885a59267477c6ec13))
* **docs:** document draft validation behavior ([#511](https://github.com/AndrewM-F/code-foundry/issues/511)) ([3526283](https://github.com/AndrewM-F/code-foundry/commit/3526283424a99f422ca28d50b3bb7c10b83e07be))
* **doctor:** accept no-CodeQL validation callers ([#509](https://github.com/AndrewM-F/code-foundry/issues/509)) ([42594f7](https://github.com/AndrewM-F/code-foundry/commit/42594f70713af5fcb248afa14240f04f2ff46c40))
* **doctor:** honor shared config and correctly identify npm/Yarn lockfiles ([#533](https://github.com/AndrewM-F/code-foundry/issues/533)) ([39d670d](https://github.com/AndrewM-F/code-foundry/commit/39d670d0b1b94929745755288b9bc8b73aa6066f))
* **doctor:** support nested Rust crates ([#525](https://github.com/AndrewM-F/code-foundry/issues/525)) ([b7a044c](https://github.com/AndrewM-F/code-foundry/commit/b7a044c3df47bbafb235abcbfc6e59ab39f402e1))
* **draft-guard:** grant draft-mutation permission and respect same-second ready transitions ([d89d8f0](https://github.com/AndrewM-F/code-foundry/commit/d89d8f058c180d9409480e08cea9b3151edd4a6b))
* draft-pr base main for direct workflow (staging deleted) ([295d611](https://github.com/AndrewM-F/code-foundry/commit/295d611ca61f792c0284c67fea2671a820adb923))
* **draft-pr:** fall back to workflow token ([#350](https://github.com/AndrewM-F/code-foundry/issues/350)) ([ee24c79](https://github.com/AndrewM-F/code-foundry/commit/ee24c7907c77e02a42aa2ea5b6d0f9d34a323f62))
* **fleet:** accept base-config evidence for merged rollouts ([#620](https://github.com/AndrewM-F/code-foundry/issues/620)) ([3508c17](https://github.com/AndrewM-F/code-foundry/commit/3508c177acd32934c30f1b8647e0c270f656ca17))
* **fleet:** bound rendered jobs with timeouts and refresh stale runtime pins ([#616](https://github.com/AndrewM-F/code-foundry/issues/616)) ([989bfc4](https://github.com/AndrewM-F/code-foundry/commit/989bfc4c7e73a275e2970bef4e32415dda7ace1f))
* **fleet:** require explicit inventory manifest ([#603](https://github.com/AndrewM-F/code-foundry/issues/603)) ([c100efd](https://github.com/AndrewM-F/code-foundry/commit/c100efdec56b4feddd2baff68290edc86acab15f))
* give the release artifact budgets several releases of headroom ([#696](https://github.com/AndrewM-F/code-foundry/issues/696)) ([44a049a](https://github.com/AndrewM-F/code-foundry/commit/44a049abc352b91fd7bacef5bfd00ffcb2c2816a))
* handle empty security audit matrices ([#785](https://github.com/AndrewM-F/code-foundry/issues/785)) ([911e627](https://github.com/AndrewM-F/code-foundry/commit/911e62725f502f7a9ec0d0412f33e3b2b08b04e1))
* **hooks:** delegate the generated pre-commit hook to the runtime ([#684](https://github.com/AndrewM-F/code-foundry/issues/684)) ([9057efe](https://github.com/AndrewM-F/code-foundry/commit/9057efeb53b2d03dd11450f5b0e6ec207f36b5d5))
* **hooks:** run the gate from a local dependency, not npx ([#688](https://github.com/AndrewM-F/code-foundry/issues/688)) ([a0bc9c4](https://github.com/AndrewM-F/code-foundry/commit/a0bc9c47761e1258b41c7c6a7f9b52d82dd9aaf9))
* keep a static check name for the Rust CodeQL job ([#462](https://github.com/AndrewM-F/code-foundry/issues/462)) ([1f6a95d](https://github.com/AndrewM-F/code-foundry/commit/1f6a95d5aa3510140c43a405b1877ddb9dfb6589))
* normalize blank runs when stripping legacy managed markers ([#678](https://github.com/AndrewM-F/code-foundry/issues/678)) ([ebc7606](https://github.com/AndrewM-F/code-foundry/commit/ebc76061a4d8e04adb96b8242fe6313a22f8d7e4))
* opt Code Foundry into source qualification receipts ([#805](https://github.com/AndrewM-F/code-foundry/issues/805)) ([bccb16f](https://github.com/AndrewM-F/code-foundry/commit/bccb16f89dd10456dea1ae74b55c79be3cbec14f))
* perf-budget-best-of-n ([#674](https://github.com/AndrewM-F/code-foundry/issues/674)) ([a90aded](https://github.com/AndrewM-F/code-foundry/commit/a90aded219cf5a6f23c1d2a897ab2ed98a734736))
* **pre-commit:** build before lint and type-check when the gate opts in ([#748](https://github.com/AndrewM-F/code-foundry/issues/748)) ([66b13bf](https://github.com/AndrewM-F/code-foundry/commit/66b13bf41976b97ce728910ad7ec0ea7761bb5d5)), closes [#691](https://github.com/AndrewM-F/code-foundry/issues/691)
* preserve consumer-only Oxc config keys across syncs ([#476](https://github.com/AndrewM-F/code-foundry/issues/476)) ([1e4b94c](https://github.com/AndrewM-F/code-foundry/commit/1e4b94c24ac5ea12081baa6dcfdb2595a14cc981))
* preserve regex escape in test assertion ([#303](https://github.com/AndrewM-F/code-foundry/issues/303)) ([8b02930](https://github.com/AndrewM-F/code-foundry/commit/8b029304a906fda5ee11468330300ebc6eb7d6fd))
* **qualification:** exclude pending parallel syntax by content, not filename ([#755](https://github.com/AndrewM-F/code-foundry/issues/755)) ([837cc19](https://github.com/AndrewM-F/code-foundry/commit/837cc19ba87b2444e1261b272cb101c524e564ae))
* **qualification:** isolate attempts and verify release handoff ([#556](https://github.com/AndrewM-F/code-foundry/issues/556)) ([86fd2b0](https://github.com/AndrewM-F/code-foundry/commit/86fd2b0f92a06ec1f818236928988b3b22353993))
* **qualification:** skip parallel-syntax files until actionlint supports them ([#740](https://github.com/AndrewM-F/code-foundry/issues/740)) ([c08ebdb](https://github.com/AndrewM-F/code-foundry/commit/c08ebdb5402758df079fce8755eff6368c7eeb04))
* **quality:** harden HTML filtering ([#562](https://github.com/AndrewM-F/code-foundry/issues/562)) ([59bbfb2](https://github.com/AndrewM-F/code-foundry/commit/59bbfb23a42373942864442780792fed684b01ae))
* recognize fixed test-and-pack receipt lifecycle ([#808](https://github.com/AndrewM-F/code-foundry/issues/808)) ([2a4dbcf](https://github.com/AndrewM-F/code-foundry/commit/2a4dbcff40799eb774c1dfc5f776d2d4ebc0e5b2))
* **reconcile:** classify final tree deltas ([#353](https://github.com/AndrewM-F/code-foundry/issues/353)) ([4b94cd8](https://github.com/AndrewM-F/code-foundry/commit/4b94cd8d824cc7170ebdeee907f30b39d136c5d9))
* **reconcile:** classify patch-equivalent trees consistently ([#360](https://github.com/AndrewM-F/code-foundry/issues/360)) ([f2eb342](https://github.com/AndrewM-F/code-foundry/commit/f2eb342dbb0839ad77f9d7710264ecc230b78ef1))
* **reconcile:** ignore historical paths absent from final tree ([#362](https://github.com/AndrewM-F/code-foundry/issues/362)) ([49612e3](https://github.com/AndrewM-F/code-foundry/commit/49612e358da1560ff41daf6d0e96183b389147de))
* release-hook-and-performance-safety ([#565](https://github.com/AndrewM-F/code-foundry/issues/565)) ([911d439](https://github.com/AndrewM-F/code-foundry/commit/911d4396c926d2f43bf55b3f06a7a89fdbea7cc1))
* release-required-check-discovery ([#392](https://github.com/AndrewM-F/code-foundry/issues/392)) ([bbf2beb](https://github.com/AndrewM-F/code-foundry/commit/bbf2bebaf4c2df0a5e1a077a0029a1825db15bc7))
* release-workspace-state ([#395](https://github.com/AndrewM-F/code-foundry/issues/395)) ([e7ea22f](https://github.com/AndrewM-F/code-foundry/commit/e7ea22fa511d30a04aa8f01c99d432a304aceb29))
* **release:** allow explicit release while CI is paused ([#407](https://github.com/AndrewM-F/code-foundry/issues/407)) ([ec525a3](https://github.com/AndrewM-F/code-foundry/commit/ec525a388c33eb2bb3bec61e9f830817e1551ab4))
* **release:** audit generated release content for stale snapshots ([#775](https://github.com/AndrewM-F/code-foundry/issues/775)) ([05bb3a8](https://github.com/AndrewM-F/code-foundry/commit/05bb3a8aa79c2d2804f311e868682477b90f9344))
* **release:** authenticate partial clone comparisons ([3b471ab](https://github.com/AndrewM-F/code-foundry/commit/3b471abd339b8b21de67cb84ee8f62234a61728d))
* **release:** automate self publication after CI ([7c2702e](https://github.com/AndrewM-F/code-foundry/commit/7c2702ed57fc9613e286aa11ca517e78c58584cf))
* **release:** avoid unsafe history-only reconciliation PRs ([#412](https://github.com/AndrewM-F/code-foundry/issues/412)) ([6537b0a](https://github.com/AndrewM-F/code-foundry/commit/6537b0ac0725fc1f03086824eba27b89e0cccc37))
* **release:** budget the package without the changelog and ship recent history only ([#708](https://github.com/AndrewM-F/code-foundry/issues/708)) ([79aed04](https://github.com/AndrewM-F/code-foundry/commit/79aed04032d826469ed24e88da7b409a832405a3))
* **release:** build exact-tree reconciliation heads ([0398a09](https://github.com/AndrewM-F/code-foundry/commit/0398a09fcb77cdd815fd9e1ecaaec08c6f04884c))
* **release:** complete rejected release-please runs over REST ([#720](https://github.com/AndrewM-F/code-foundry/issues/720)) ([755d1a8](https://github.com/AndrewM-F/code-foundry/commit/755d1a8b81ad41b0ac6a47b3e664752d3a3fee38))
* **release:** cover the attestation lag in publication retries ([#587](https://github.com/AndrewM-F/code-foundry/issues/587)) ([1a39344](https://github.com/AndrewM-F/code-foundry/commit/1a39344458d2c90569d85a0824a0290058bebeb4))
* **release:** hydrate audit blobs and refresh changing PR state ([#779](https://github.com/AndrewM-F/code-foundry/issues/779)) ([c133f2d](https://github.com/AndrewM-F/code-foundry/commit/c133f2d649b28a26d89cc6d5a5c9571a611a9ba9))
* **release:** include ssh executable in reconcile transport ([#308](https://github.com/AndrewM-F/code-foundry/issues/308)) ([8d12d85](https://github.com/AndrewM-F/code-foundry/commit/8d12d85db928f2b2656085107f90976b9cdd13cc))
* **release:** install dependencies before npm publish ([88f8d20](https://github.com/AndrewM-F/code-foundry/commit/88f8d20fbc7d35e23fda290caade995338d68a54))
* **release:** keep reconcile fetch over HTTPS ([#305](https://github.com/AndrewM-F/code-foundry/issues/305)) ([dbc79f4](https://github.com/AndrewM-F/code-foundry/commit/dbc79f4e365c260fdf1eddb693a5559ffb3c5b92))
* **release:** make batched publication and stable promotion reliable ([#703](https://github.com/AndrewM-F/code-foundry/issues/703)) ([1253a79](https://github.com/AndrewM-F/code-foundry/commit/1253a797d676172c5211f5078bb747d1a3dcdc38))
* **release:** make mergeability poll executable ([#314](https://github.com/AndrewM-F/code-foundry/issues/314)) ([9c2736f](https://github.com/AndrewM-F/code-foundry/commit/9c2736f47d60584908aacbdcd4f539398ae9af0d))
* **release:** make the REST fallback draft-aware and idempotent ([#725](https://github.com/AndrewM-F/code-foundry/issues/725)) ([788debd](https://github.com/AndrewM-F/code-foundry/commit/788debd7697c1026f29ffced304d399600112cf2))
* **release:** mirror staging onto main and require rebase merges on main ([0f9351c](https://github.com/AndrewM-F/code-foundry/commit/0f9351c5ec2475263df74ef6b5e2d8c8ecdf92bd))
* **release:** no-op when staging already points at main's commit ([c32c794](https://github.com/AndrewM-F/code-foundry/commit/c32c794a5f62dc6feccec30b33e215ac635a2bd8))
* **release:** pass one qualification report per required node ([#597](https://github.com/AndrewM-F/code-foundry/issues/597)) ([00bf673](https://github.com/AndrewM-F/code-foundry/commit/00bf6736aae7ed1684a9320389b6a6b8835b0970))
* **release:** preserve current-head validation ownership ([#737](https://github.com/AndrewM-F/code-foundry/issues/737)) ([be24e2c](https://github.com/AndrewM-F/code-foundry/commit/be24e2c341990bf99d75874bb7181b54002bdc39))
* **release:** preserve fallback stdin and paginate existing releases ([#781](https://github.com/AndrewM-F/code-foundry/issues/781)) ([921f0b5](https://github.com/AndrewM-F/code-foundry/commit/921f0b5d61db7f236dbff45a0131a7679654f140))
* **release:** preserve promotion release semantics ([#418](https://github.com/AndrewM-F/code-foundry/issues/418)) ([8db8a7d](https://github.com/AndrewM-F/code-foundry/commit/8db8a7d5148962e1a26410351ba350ed4c517b8a))
* **release:** probe the tag-creation write before trusting the automation token ([#716](https://github.com/AndrewM-F/code-foundry/issues/716)) ([9dcda7e](https://github.com/AndrewM-F/code-foundry/commit/9dcda7e618adfbe0e163005e2826e95ab7108ffc))
* **release:** provision bun and corepack before publish install ([065b4c3](https://github.com/AndrewM-F/code-foundry/commit/065b4c3b7185f8ef0c3bdb1720a266234ec170dc))
* **release:** qualify promotion PR head filters ([b74cc21](https://github.com/AndrewM-F/code-foundry/commit/b74cc21fe35737028f2fb78d98452dd0fc868934))
* **release:** query the version-PR branch directly in the REST fallback ([#722](https://github.com/AndrewM-F/code-foundry/issues/722)) ([111e1ef](https://github.com/AndrewM-F/code-foundry/commit/111e1ef9e54c3527088e3f9dea8e5a2f9a8868a9))
* **release:** queue version PR merges on branch policy ([#646](https://github.com/AndrewM-F/code-foundry/issues/646)) ([a8994ae](https://github.com/AndrewM-F/code-foundry/commit/a8994aef1b5189c6a3df2368c41a6a0627bda284))
* **release:** reconcile only after creating a release ([#317](https://github.com/AndrewM-F/code-foundry/issues/317)) ([#318](https://github.com/AndrewM-F/code-foundry/issues/318)) ([290e27f](https://github.com/AndrewM-F/code-foundry/commit/290e27f5ac7c849fedd0bc4cdc45e1d76fce8379))
* **release:** reconcile protected staging branches ([871db4d](https://github.com/AndrewM-F/code-foundry/commit/871db4d48cf70be07d27c11cb490e657cb3b3894))
* **release:** retry integrity verification through the publication consistency window ([#585](https://github.com/AndrewM-F/code-foundry/issues/585)) ([11a7296](https://github.com/AndrewM-F/code-foundry/commit/11a7296700bf486c7a8da7604770f149d5da13b9))
* **release:** retry the token probe and REST fallback writes with backoff ([#729](https://github.com/AndrewM-F/code-foundry/issues/729)) ([ec28eaa](https://github.com/AndrewM-F/code-foundry/commit/ec28eaa6856f96d164d2952d14b8f11151fa0688))
* **release:** scope reconciliation to staging topology ([152ebd4](https://github.com/AndrewM-F/code-foundry/commit/152ebd4207dff682800354e455fcbf167e96bc97))
* **release:** squash Release Please PRs for release-please compatibility ([85be623](https://github.com/AndrewM-F/code-foundry/commit/85be6237c6ed9375553cc5aa93243714a01bdade))
* **release:** squash release PRs so staging can fast-forward after releases ([9f4c942](https://github.com/AndrewM-F/code-foundry/commit/9f4c942c2420017bb1651a47472a1a01c99e16f5))
* **release:** stop version pull requests from closing referenced issues ([#833](https://github.com/AndrewM-F/code-foundry/issues/833)) ([8a843e3](https://github.com/AndrewM-F/code-foundry/commit/8a843e3ff3abe97680e79e5a5ff7cf63cc402d5b))
* **release:** sync bun.lock workspace versions on generated release PRs ([#777](https://github.com/AndrewM-F/code-foundry/issues/777)) ([aa32e94](https://github.com/AndrewM-F/code-foundry/commit/aa32e944a07d506445f160627e623281587186e2))
* **release:** synchronize staging with a linear commit instead of a blocked fast-forward ([6d50015](https://github.com/AndrewM-F/code-foundry/commit/6d500151afcf4f93b7b80bc671d44f9ae6132fc0))
* **release:** treat ref-creation errors in the REST fallback as non-fatal ([#727](https://github.com/AndrewM-F/code-foundry/issues/727)) ([3a2f265](https://github.com/AndrewM-F/code-foundry/commit/3a2f2654868400c529829734767dd4b7a5c1fad2))
* **release:** unblock draft publication and PR deployment links ([#570](https://github.com/AndrewM-F/code-foundry/issues/570)) ([010d286](https://github.com/AndrewM-F/code-foundry/commit/010d286d2aff711e0e2bcd2149505d15f6d51639))
* **release:** use rebase for release PRs ([#358](https://github.com/AndrewM-F/code-foundry/issues/358)) ([3a0bc8b](https://github.com/AndrewM-F/code-foundry/commit/3a0bc8b631d1613ed827dbb8351a3c313ee184fb))
* **release:** use shell-safe recovery script ([#574](https://github.com/AndrewM-F/code-foundry/issues/574)) ([8aed0cb](https://github.com/AndrewM-F/code-foundry/commit/8aed0cbd49eb34aacb98f3dff0fa953cc4036b66))
* **release:** validate automation token before Release Please ([bf28e84](https://github.com/AndrewM-F/code-foundry/commit/bf28e84d6260830b0749a030c5b08812afa77802))
* **release:** wait for PR mergeability before guarded auto-merge ([#311](https://github.com/AndrewM-F/code-foundry/issues/311)) ([a81f55d](https://github.com/AndrewM-F/code-foundry/commit/a81f55db9d49cb68b106f3f99b7a0584a794b813))
* **release:** wait for the release index before verifying a published release ([#583](https://github.com/AndrewM-F/code-foundry/issues/583)) ([5f2a734](https://github.com/AndrewM-F/code-foundry/commit/5f2a734855bfa870543d7bc7b988c8fd2a665b44))
* **release:** wait for the synchronize validation run before re-readying ([#829](https://github.com/AndrewM-F/code-foundry/issues/829)) ([130996e](https://github.com/AndrewM-F/code-foundry/commit/130996ebc506ca4c23aa5a2e525d64b3a33866b3))
* report inactive main rulesets in github doctor ([#682](https://github.com/AndrewM-F/code-foundry/issues/682)) ([f5ad8be](https://github.com/AndrewM-F/code-foundry/commit/f5ad8bed4fc542be64512ec142bbccfcbf6460fa))
* require candidate asset qualification before stable promotion ([#705](https://github.com/AndrewM-F/code-foundry/issues/705)) ([7e92336](https://github.com/AndrewM-F/code-foundry/commit/7e9233686c5fef00773bd695b865afb381de1293))
* restore job-level OpenCode scanner call; preserve consumer oxlint ignores on sync ([#473](https://github.com/AndrewM-F/code-foundry/issues/473)) ([42657ca](https://github.com/AndrewM-F/code-foundry/commit/42657ca9ba4a1f7447f2876384b2d2ba45078b35))
* restore pre-matrix CodeQL SARIF category strings ([#468](https://github.com/AndrewM-F/code-foundry/issues/468)) ([61ffc7d](https://github.com/AndrewM-F/code-foundry/commit/61ffc7ddebc1d35f49440232c0c2d77d2fefe0dd))
* restore source qualification receipt reuse ([#801](https://github.com/AndrewM-F/code-foundry/issues/801)) ([ff55a6a](https://github.com/AndrewM-F/code-foundry/commit/ff55a6a916bf331b62306a380b101e0fc3b1b958))
* retry transient release fallback reads safely ([#800](https://github.com/AndrewM-F/code-foundry/issues/800)) ([0b674b4](https://github.com/AndrewM-F/code-foundry/commit/0b674b43bc14e510a6219d70fc9f2bf6319e2645))
* safely categorize npm publication failures ([#787](https://github.com/AndrewM-F/code-foundry/issues/787)) ([03724b8](https://github.com/AndrewM-F/code-foundry/commit/03724b8b8229c9e88e09655cce0d6f5551c9dde0))
* save repository caches through an explicit save action ([#819](https://github.com/AndrewM-F/code-foundry/issues/819)) ([8282e3c](https://github.com/AndrewM-F/code-foundry/commit/8282e3c927fc6ecee4b9ea8494d8e592bcdfc951))
* scope dependabot ecosystems to configured languages ([#457](https://github.com/AndrewM-F/code-foundry/issues/457)) ([fc432e9](https://github.com/AndrewM-F/code-foundry/commit/fc432e969fb58bdbfcfd42d27ece480991b33861))
* scope draft cancellation to its pull request ([#799](https://github.com/AndrewM-F/code-foundry/issues/799)) ([de5f1e6](https://github.com/AndrewM-F/code-foundry/commit/de5f1e66ea15c5822449e3d23e678ce31f25bc7e))
* **security:** only save caches on push in security workflow ([20fe09b](https://github.com/AndrewM-F/code-foundry/commit/20fe09b08545d6287e9c012c28d1672354ea395f))
* **security:** pin authoritative scan resealing ([1c0dcb7](https://github.com/AndrewM-F/code-foundry/commit/1c0dcb754ee1ae53fe8363440935f6e7d9d2993d))
* **security:** pin scanner target normalization ([ac5b745](https://github.com/AndrewM-F/code-foundry/commit/ac5b7458b8b7f37aed43cf67b8bce37c24ec8408))
* **security:** pin scheduled audit runtime ([#491](https://github.com/AndrewM-F/code-foundry/issues/491)) ([3e1add2](https://github.com/AndrewM-F/code-foundry/commit/3e1add29a4d04a284c487bf3beac7db1ba864bcf))
* **security:** remove cache-capable setup from audits ([#489](https://github.com/AndrewM-F/code-foundry/issues/489)) ([a76a3df](https://github.com/AndrewM-F/code-foundry/commit/a76a3dfdd07ba898200fdff40bfa4826b2b37390))
* **security:** save caches on push events only ([e39efad](https://github.com/AndrewM-F/code-foundry/commit/e39efade3385b3acafdefce6076e7c871501c094))
* **security:** stop a clean pip-audit result from failing the audit gate ([#643](https://github.com/AndrewM-F/code-foundry/issues/643)) ([926901c](https://github.com/AndrewM-F/code-foundry/commit/926901c10f117a1ed14919f972a0f888d8c7a15b))
* split native test suites by category ([d271da0](https://github.com/AndrewM-F/code-foundry/commit/d271da0f10de46247c706b0c17ec52e3e4e3ea24))
* support reviewed Playwright 1.64.1 UI receipts ([#817](https://github.com/AndrewM-F/code-foundry/issues/817)) ([cce1fe2](https://github.com/AndrewM-F/code-foundry/commit/cce1fe2b337498d92f472a4477ce17c3eccf23d9))
* sync-caller-runtime-pin ([#484](https://github.com/AndrewM-F/code-foundry/issues/484)) ([a9d1eda](https://github.com/AndrewM-F/code-foundry/commit/a9d1edae5a25c48fee4a2bc07d2ce18c98f5bc46))
* **sync:** accept mixed broad and scoped CodeQL Rust shards ([#621](https://github.com/AndrewM-F/code-foundry/issues/621)) ([aec4788](https://github.com/AndrewM-F/code-foundry/commit/aec478858b3d0050b32447a1d207f8cac84ee5ef))
* **sync:** chain machine-level hooks instead of silencing them ([#747](https://github.com/AndrewM-F/code-foundry/issues/747)) ([d6b9da8](https://github.com/AndrewM-F/code-foundry/commit/d6b9da85561d605864b2bb94595f560c24ded2f9)), closes [#690](https://github.com/AndrewM-F/code-foundry/issues/690)
* **sync:** hold TypeScript toolchain below v7 in consumer dependabot config ([c686bdd](https://github.com/AndrewM-F/code-foundry/commit/c686bdd6482357aa661e0251fd31b67e921841d3))
* **sync:** keep prettier ignores idempotent ([29ef25c](https://github.com/AndrewM-F/code-foundry/commit/29ef25ca676baa6b41439ee88ad51e418754e44c))
* **sync:** never leak runtime release-type into consumer configs ([78d9071](https://github.com/AndrewM-F/code-foundry/commit/78d90712ffba9e7f98edbfccfe667be267b10723))
* **sync:** omit Cargo Dependabot outside Rust repos ([#398](https://github.com/AndrewM-F/code-foundry/issues/398)) ([5466d77](https://github.com/AndrewM-F/code-foundry/commit/5466d775ac5296cffb807c31789b76055fd8512b))
* **sync:** preserve non-CodeQL workflow triggers ([#605](https://github.com/AndrewM-F/code-foundry/issues/605)) ([b5793d8](https://github.com/AndrewM-F/code-foundry/commit/b5793d89439f7d4cfd1e3105f378a9a53e97b272))
* **sync:** prettier-canonical CONTRIBUTING.md tables for both topologies ([94d03d0](https://github.com/AndrewM-F/code-foundry/commit/94d03d094e701d69e45abe0f90da6278c3d478e4))
* **sync:** prettier-canonical dependabot ignore quotes ([587e782](https://github.com/AndrewM-F/code-foundry/commit/587e7826d56324039febc4a3f6842197faf6244b))
* **sync:** prettier-canonical direct doc tables + dependabot ignore for runtime pins ([432b06f](https://github.com/AndrewM-F/code-foundry/commit/432b06f83c47a022864bafa58fd56ae9699e04bf))
* **sync:** quote collection-like config values so prettier accepts them ([f6d9460](https://github.com/AndrewM-F/code-foundry/commit/f6d94603c6de1dc2696e279e85a70b02a9cb5ad2))
* **sync:** refresh config-aware policies ([#505](https://github.com/AndrewM-F/code-foundry/issues/505)) ([1a73d66](https://github.com/AndrewM-F/code-foundry/commit/1a73d662163009b0ea056504c917c504864c3ff4))
* **sync:** remove direct topology staging residue ([#515](https://github.com/AndrewM-F/code-foundry/issues/515)) ([c7ea4b5](https://github.com/AndrewM-F/code-foundry/commit/c7ea4b50998a7610cc1beeb71e786b29dc268dfa))
* **sync:** render the configured Rust shards into every CodeQL lane ([#612](https://github.com/AndrewM-F/code-foundry/issues/612)) ([3e282b8](https://github.com/AndrewM-F/code-foundry/commit/3e282b818de0a3146b1947a7c0b76a3bc9c5bf3e))
* **sync:** replace complete consumer runtime ref ([#793](https://github.com/AndrewM-F/code-foundry/issues/793)) ([aa7de9e](https://github.com/AndrewM-F/code-foundry/commit/aa7de9e13397a97c78f77b8ef4ee04a4af529463))
* **sync:** satisfy JSDoc type-check for baseline merge ([fcb570c](https://github.com/AndrewM-F/code-foundry/commit/fcb570c4646580b493b869a91ad5a5319e0ac1ee))
* **sync:** standardize existing release PR titles ([#521](https://github.com/AndrewM-F/code-foundry/issues/521)) ([51ac40c](https://github.com/AndrewM-F/code-foundry/commit/51ac40c2473485c41fd5ee75f90d2e7b36999c7b))
* validate license policy before sync ([0f8f4a5](https://github.com/AndrewM-F/code-foundry/commit/0f8f4a5650a00e41bcbad34f29f57278a92572dd))
* validation-issue-read-v1471 ([#759](https://github.com/AndrewM-F/code-foundry/issues/759)) ([ddf7f1c](https://github.com/AndrewM-F/code-foundry/commit/ddf7f1c8c9222cc4258e581e3aed9ba6040091cd))
* **validation:** load consumer audit policy ([294c7e1](https://github.com/AndrewM-F/code-foundry/commit/294c7e1d66925aad2912d58a9bfb0406f8f0238e))
* **validation:** run available suites for no-CodeQL releases ([122af66](https://github.com/AndrewM-F/code-foundry/commit/122af66c08645e2623d3f250597884cb16749236))
* **validation:** run CodeQL on the release tier ([6947741](https://github.com/AndrewM-F/code-foundry/commit/694774186b8b0791707a8fcb264b3016334c8e43))
* **validation:** scan default branch with CodeQL on push ([#540](https://github.com/AndrewM-F/code-foundry/issues/540)) ([8cb8b49](https://github.com/AndrewM-F/code-foundry/commit/8cb8b49779e44dc80d736c3223616de49636d184))
* **validation:** skip eslint fallback without repo setup and ignore overlaid actions ([d926d5d](https://github.com/AndrewM-F/code-foundry/commit/d926d5d07b5f1e4ca1cdb2d06c7ebf0b56ff48fe))
* vite-plus-cache-post-job-save ([#765](https://github.com/AndrewM-F/code-foundry/issues/765)) ([fb8746c](https://github.com/AndrewM-F/code-foundry/commit/fb8746cf6512ac1e97f16c768fd03c8a81b53c1f))
* **workflows:** disable security cache writes ([#487](https://github.com/AndrewM-F/code-foundry/issues/487)) ([0238801](https://github.com/AndrewM-F/code-foundry/commit/0238801cdbac89202dbc2af7e120aa35915bd3f2))


### Performance

* **ci:** batch native Rust test targets by category ([#564](https://github.com/AndrewM-F/code-foundry/issues/564)) ([6073028](https://github.com/AndrewM-F/code-foundry/commit/6073028981b3edd855ee99b46a5e2b8f87e5f3ca))
* **ci:** run mixed unit runners concurrently ([#821](https://github.com/AndrewM-F/code-foundry/issues/821)) ([ad90944](https://github.com/AndrewM-F/code-foundry/commit/ad9094401f45f2ef5272aa630bb29f98f0cff719))
* **codeql:** drop unchanged analyzers from the planned matrix ([#831](https://github.com/AndrewM-F/code-foundry/issues/831)) ([470ae28](https://github.com/AndrewM-F/code-foundry/commit/470ae28d50d7f2e3c0e2bc81c715c2f43490ba2d))
* **validation:** fold Security Profile and CodeQL Detect into the plan job ([#827](https://github.com/AndrewM-F/code-foundry/issues/827)) ([0f66686](https://github.com/AndrewM-F/code-foundry/commit/0f6668600a72ac9f6d258e342a77147ddf2e858e))
* **validation:** skip lane jobs that have nothing to run ([#825](https://github.com/AndrewM-F/code-foundry/issues/825)) ([a234f95](https://github.com/AndrewM-F/code-foundry/commit/a234f95cae07236fbede8e8a908cad7aa0c300e8))


### Documentation

* **agents:** use GitButler and stop creating worktrees ([#842](https://github.com/AndrewM-F/code-foundry/issues/842)) ([a87b2c9](https://github.com/AndrewM-F/code-foundry/commit/a87b2c9656161878c88fa22f7111d4a39fb2fdae))
* fix generated agent contribution and validation references ([#760](https://github.com/AndrewM-F/code-foundry/issues/760)) ([e04e627](https://github.com/AndrewM-F/code-foundry/commit/e04e62704018e624034fc2ca892b5caa793adab4))
* refresh documentation for current workflows ([#568](https://github.com/AndrewM-F/code-foundry/issues/568)) ([c7fabf9](https://github.com/AndrewM-F/code-foundry/commit/c7fabf9b20df6d5503339e585bbfbbd534cfc750))
* **sync:** align release validation guidance ([#518](https://github.com/AndrewM-F/code-foundry/issues/518)) ([571a837](https://github.com/AndrewM-F/code-foundry/commit/571a83727cbe25e7227c624c4116363860f12321))


### Tests

* **cli:** assert expected doctor warnings ([#712](https://github.com/AndrewM-F/code-foundry/issues/712)) ([257a564](https://github.com/AndrewM-F/code-foundry/commit/257a5643bdd54b410a5f74c711cb9e9d7143ce9f))
* **doctor:** pin the machine-hook shadow warning ([#753](https://github.com/AndrewM-F/code-foundry/issues/753)) ([0567fd1](https://github.com/AndrewM-F/code-foundry/commit/0567fd1ff92efc84936cd5e81abd8fd33af339ce))
* expect quoted codeql_rust_shards in generated config ([3b765bd](https://github.com/AndrewM-F/code-foundry/commit/3b765bd9e06b929adce2a49c254cc68dfe6a1aac))
* read the chained hook fixture with fs.readFileSync ([#769](https://github.com/AndrewM-F/code-foundry/issues/769)) ([b289ef9](https://github.com/AndrewM-F/code-foundry/commit/b289ef96baa5a99b93f8e6695d5b83a501a7bb3f))
* tolerate runner contention in readiness fixtures ([#836](https://github.com/AndrewM-F/code-foundry/issues/836)) ([b0cdaf7](https://github.com/AndrewM-F/code-foundry/commit/b0cdaf72d4d18df5c4eca18645fa5c88883ecb34))


### CI

* split Dependabot security updates ([#356](https://github.com/AndrewM-F/code-foundry/issues/356)) ([e791d71](https://github.com/AndrewM-F/code-foundry/commit/e791d7141d5f8875cc83c97a13d6ab3b5d02ec37))
* **validation:** require release checks until evidence exists ([#789](https://github.com/AndrewM-F/code-foundry/issues/789)) ([8637a6a](https://github.com/AndrewM-F/code-foundry/commit/8637a6a8ce5c0dfbb2ea764a2c6b11aa5afdd347))


### Maintenance

* add verified npm publication recovery ([#815](https://github.com/AndrewM-F/code-foundry/issues/815)) ([033163c](https://github.com/AndrewM-F/code-foundry/commit/033163cddcb5d79634e21cc63d95cfab172c3bbf))
* adopt Code Foundry runtime v1.30.0 ([#634](https://github.com/AndrewM-F/code-foundry/issues/634)) ([747581d](https://github.com/AndrewM-F/code-foundry/commit/747581dc79405a24f81df724905b531659204010))
* align oxlint and oxfmt pins with fleet standard ([#628](https://github.com/AndrewM-F/code-foundry/issues/628)) ([86c2af8](https://github.com/AndrewM-F/code-foundry/commit/86c2af8fac308b341364c4a8cf3a9974e1fbaf9c))
* align self-hosted runtime reference ([#323](https://github.com/AndrewM-F/code-foundry/issues/323)) ([9175343](https://github.com/AndrewM-F/code-foundry/commit/9175343a1eedf817f4d82553e8698692af840a19))
* bump runtime ref and release config to manifest mode ([028e589](https://github.com/AndrewM-F/code-foundry/commit/028e58941e2360438f73be7615d2c2c3df3998e0))
* bun-1.4.4-cloud ([#771](https://github.com/AndrewM-F/code-foundry/issues/771)) ([4777196](https://github.com/AndrewM-F/code-foundry/commit/477719676e20dbf65703c3514978e3d9b50537a0))
* **bun:** align Bun runtime pins to 1.4.3 ([#767](https://github.com/AndrewM-F/code-foundry/issues/767)) ([4e6bdfe](https://github.com/AndrewM-F/code-foundry/commit/4e6bdfef6c980bba84a7ff7363abefcd659c9f8e))
* **ci:** dogfood runtime v1.0.0 in self workflows ([5a5455d](https://github.com/AndrewM-F/code-foundry/commit/5a5455dc1ca920f0dcb6bec1accc6b45d6821d54))
* **ci:** dogfood runtime v1.0.4 in self workflows ([18df122](https://github.com/AndrewM-F/code-foundry/commit/18df122aa9f96a51211c9775ffad59f9b93dbeae))
* **ci:** dogfood runtime v1.0.5 in self workflows ([#456](https://github.com/AndrewM-F/code-foundry/issues/456)) ([2c5f9e9](https://github.com/AndrewM-F/code-foundry/commit/2c5f9e9500c1f06fc45fd47006aaa34506a0bad3))
* **ci:** dogfood runtime v1.1.0 in self workflows ([#461](https://github.com/AndrewM-F/code-foundry/issues/461)) ([46d2c49](https://github.com/AndrewM-F/code-foundry/commit/46d2c4995bad34b96e087df3206aa28abcb0b31a))
* **ci:** dogfood runtime v1.1.1 in self workflows ([#464](https://github.com/AndrewM-F/code-foundry/issues/464)) ([bfebd7c](https://github.com/AndrewM-F/code-foundry/commit/bfebd7c536ac825e98cd98cd8f882dcc38fe046a))
* **ci:** dogfood runtime v1.2.0 in self workflows ([#467](https://github.com/AndrewM-F/code-foundry/issues/467)) ([53e49ce](https://github.com/AndrewM-F/code-foundry/commit/53e49cee5ff2c02a03f3f0e1ca404af588175615))
* **ci:** dogfood runtime v1.3.1 in self workflows ([#475](https://github.com/AndrewM-F/code-foundry/issues/475)) ([f542fa4](https://github.com/AndrewM-F/code-foundry/commit/f542fa45a96155e301fbba71a215ee67fd27ffe2))
* complete direct-workflow schema keys in code-foundry config ([#453](https://github.com/AndrewM-F/code-foundry/issues/453)) ([f3f8764](https://github.com/AndrewM-F/code-foundry/commit/f3f876453e67c846635d3963551d075c7071f27b))
* **config:** pin Code Foundry runtime to v1.28.2 ([#599](https://github.com/AndrewM-F/code-foundry/issues/599)) ([cd6475a](https://github.com/AndrewM-F/code-foundry/commit/cd6475a1fa10a01b3d952d08d7ace8c43eacdff7))
* **deps:** bump the github-actions group with 5 updates ([#376](https://github.com/AndrewM-F/code-foundry/issues/376)) ([6607f3a](https://github.com/AndrewM-F/code-foundry/commit/6607f3a32755c7bb4f75990c50e39bfa805aa1e7))
* **deps:** update Code Foundry toolchain ([#310](https://github.com/AndrewM-F/code-foundry/issues/310)) ([b1dec8e](https://github.com/AndrewM-F/code-foundry/commit/b1dec8e0605a9a3fee6c2f2c2a829f0f5c8c7aad))
* **fleet:** add explicit inventory manifest ([#618](https://github.com/AndrewM-F/code-foundry/issues/618)) ([419005b](https://github.com/AndrewM-F/code-foundry/commit/419005b5cac9a5bcf557afbd8c4c5f91664e5cba))
* **fleet:** point the manifest at the rollout worktrees and filter adea's actionlint ([#757](https://github.com/AndrewM-F/code-foundry/issues/757)) ([cf68776](https://github.com/AndrewM-F/code-foundry/commit/cf68776f4af4a36d8ee6f62b112bee821ad8c1fe))
* **main:** release 0.32.1 ([#293](https://github.com/AndrewM-F/code-foundry/issues/293)) ([93a6e57](https://github.com/AndrewM-F/code-foundry/commit/93a6e575407e07e130e00d058f2678fa0e6708d1))
* **main:** release 0.32.2 ([30af381](https://github.com/AndrewM-F/code-foundry/commit/30af381e8a5b76cbe14f863d49c7349190046df4))
* **main:** release 0.32.3 ([#298](https://github.com/AndrewM-F/code-foundry/issues/298)) ([49c8d89](https://github.com/AndrewM-F/code-foundry/commit/49c8d898f686517e0ee7e9bc7c471622d89b88da))
* **main:** release 0.32.4 ([#300](https://github.com/AndrewM-F/code-foundry/issues/300)) ([5efce6e](https://github.com/AndrewM-F/code-foundry/commit/5efce6ecd298170d372863c71a4d4fc27e0dedc5))
* **main:** release 0.33.0 ([#304](https://github.com/AndrewM-F/code-foundry/issues/304)) ([6c8bc9a](https://github.com/AndrewM-F/code-foundry/commit/6c8bc9a2d9159d812ef7955d86e34e9721088a9b))
* **main:** release 0.34.0 ([#309](https://github.com/AndrewM-F/code-foundry/issues/309)) ([58472b8](https://github.com/AndrewM-F/code-foundry/commit/58472b83a1c4919727960b034af9f1a00b3cf7a0))
* **main:** release 0.34.1 ([#313](https://github.com/AndrewM-F/code-foundry/issues/313)) ([d9f5c98](https://github.com/AndrewM-F/code-foundry/commit/d9f5c982861ce2fb281212fe8cd63f214d3a2b34))
* **main:** release 0.34.10 ([#349](https://github.com/AndrewM-F/code-foundry/issues/349)) ([149600a](https://github.com/AndrewM-F/code-foundry/commit/149600acfcba988b763dd7e2e828d8443f906a33))
* **main:** release 0.34.11 ([#352](https://github.com/AndrewM-F/code-foundry/issues/352)) ([1b1de3f](https://github.com/AndrewM-F/code-foundry/commit/1b1de3fd4d511d4cd1093adbecd7ca1f5dd8eb8f))
* **main:** release 0.34.12 ([#355](https://github.com/AndrewM-F/code-foundry/issues/355)) ([ccf70b3](https://github.com/AndrewM-F/code-foundry/commit/ccf70b368a7bad7adcac28ee06e7f40d31b85224))
* **main:** release 0.34.13 ([f1453ba](https://github.com/AndrewM-F/code-foundry/commit/f1453ba5d501d208b4aff924d293fc5df67a961b))
* **main:** release 0.34.14 ([a16bb78](https://github.com/AndrewM-F/code-foundry/commit/a16bb780886dacb7ef975cb3e6fe3b024c3fc038))
* **main:** release 0.34.2 ([#316](https://github.com/AndrewM-F/code-foundry/issues/316)) ([75043e5](https://github.com/AndrewM-F/code-foundry/commit/75043e595e8a737d0c6432b077d8fe1ae8e7d9e3))
* **main:** release 0.34.3 ([#319](https://github.com/AndrewM-F/code-foundry/issues/319)) ([695f22a](https://github.com/AndrewM-F/code-foundry/commit/695f22a835c3d77fb5fbbd21c9c6fa995c69694c))
* **main:** release 0.34.4 ([#322](https://github.com/AndrewM-F/code-foundry/issues/322)) ([fe0fb84](https://github.com/AndrewM-F/code-foundry/commit/fe0fb84de51d706b453bf054331fee5a8cfb38ad))
* **main:** release 0.34.5 ([#327](https://github.com/AndrewM-F/code-foundry/issues/327)) ([ec86622](https://github.com/AndrewM-F/code-foundry/commit/ec86622d5584179a94edae3b6383ed72814cb03c))
* **main:** release 0.34.6 ([#330](https://github.com/AndrewM-F/code-foundry/issues/330)) ([d71b3f4](https://github.com/AndrewM-F/code-foundry/commit/d71b3f4bf80f133ebc69280c7a0c12ce629b326d))
* **main:** release 0.34.7 ([#333](https://github.com/AndrewM-F/code-foundry/issues/333)) ([e7f335b](https://github.com/AndrewM-F/code-foundry/commit/e7f335b9ea2eeaa62ddcdba8cb419cd1f17afdb3))
* **main:** release 0.34.8 ([#342](https://github.com/AndrewM-F/code-foundry/issues/342)) ([f9adcb7](https://github.com/AndrewM-F/code-foundry/commit/f9adcb795b76532704dc256f62db793c47fc3016))
* **main:** release 0.34.9 ([#345](https://github.com/AndrewM-F/code-foundry/issues/345)) ([e66d0b4](https://github.com/AndrewM-F/code-foundry/commit/e66d0b4045e2b4efa27a530ec5497771290a6399))
* **main:** release 0.35.0 ([d02e1d6](https://github.com/AndrewM-F/code-foundry/commit/d02e1d6b333d0eda99911bfc7591000889e6817a))
* **main:** release 0.36.0 ([3753ec1](https://github.com/AndrewM-F/code-foundry/commit/3753ec184c79405bf4305098588baaf0e0a1f878))
* **main:** release 0.36.1 ([63060b2](https://github.com/AndrewM-F/code-foundry/commit/63060b2aee8d2c691aee5e6cc79c2caa19414900))
* **main:** release 0.36.2 ([b934d73](https://github.com/AndrewM-F/code-foundry/commit/b934d73fdfcbdc6d5b47e1c9a942a089a732fdd3))
* **main:** release 0.37.0 ([608de88](https://github.com/AndrewM-F/code-foundry/commit/608de884e0ff8d00f78041e0a7173a293b5464c6))
* **main:** release 0.37.1 ([c6e1c13](https://github.com/AndrewM-F/code-foundry/commit/c6e1c13f6b08a8a6d2b87dfd1ec4ad4ee5fee55a))
* **main:** release 0.37.2 ([97cbeef](https://github.com/AndrewM-F/code-foundry/commit/97cbeefbb0f617bef2e5ef4de752ad89a82051b4))
* **main:** release 0.37.3 ([77ee5a5](https://github.com/AndrewM-F/code-foundry/commit/77ee5a57e40b9c04c7ab589ca59854fee80ad5ff))
* **main:** release 0.37.4 ([49e7c69](https://github.com/AndrewM-F/code-foundry/commit/49e7c69b8e6fa07e6ca28ab054797c10967e3de6))
* **main:** release 0.37.5 ([6471e80](https://github.com/AndrewM-F/code-foundry/commit/6471e80dafec940d7332da81f05fca3846e9b7d1))
* **main:** release 0.38.0 ([a53f2c4](https://github.com/AndrewM-F/code-foundry/commit/a53f2c4d1cdce1a856a6826e2dacff610665cb83))
* **main:** release 0.38.1 ([9062c7f](https://github.com/AndrewM-F/code-foundry/commit/9062c7f31ed5cc0579b772ad2007bc64934c419f))
* **main:** release 0.38.2 ([f95cde1](https://github.com/AndrewM-F/code-foundry/commit/f95cde128a9a9f870ec8cfaacc8d51e88dfd0e11))
* **main:** release 0.39.0 ([24de8be](https://github.com/AndrewM-F/code-foundry/commit/24de8be6e7be1c44779bfad3e42944e847b67459))
* **main:** release 0.39.1 ([62b7ee0](https://github.com/AndrewM-F/code-foundry/commit/62b7ee002b625c922f6135605b34c34b18f315a7))
* **main:** release 0.39.2 ([fdf455a](https://github.com/AndrewM-F/code-foundry/commit/fdf455a2fe922222e4846f0515e68adc74c7de67))
* **main:** release 0.39.3 ([1c477ff](https://github.com/AndrewM-F/code-foundry/commit/1c477ff55ec613c2542784c46c7fd6a157e2fa37))
* **main:** release 0.39.4 ([d6d3bcf](https://github.com/AndrewM-F/code-foundry/commit/d6d3bcf3376ea933151ae76eee0b74d0193e3c97))
* **main:** release 0.40.0 ([e0c7ab8](https://github.com/AndrewM-F/code-foundry/commit/e0c7ab807fd5ce61192728681c7956695419a00c))
* **main:** release 0.40.1 ([7b186e6](https://github.com/AndrewM-F/code-foundry/commit/7b186e6f2776a08d25bdbfc72b38292aeca2f619))
* **main:** release 0.40.2 ([4bf1846](https://github.com/AndrewM-F/code-foundry/commit/4bf184644fde417fb20931349410e18e7e824a6e))
* **main:** release 0.40.3 ([25b1db5](https://github.com/AndrewM-F/code-foundry/commit/25b1db58eb7b1efe033a44121061a392f5222dd4))
* **main:** release 1.0.0 ([cd22aea](https://github.com/AndrewM-F/code-foundry/commit/cd22aeadb1370a0beb42e4be0d3ecc3dc61d17ef))
* **main:** release 1.0.1 ([b70fb05](https://github.com/AndrewM-F/code-foundry/commit/b70fb0510034ea0d7b07aaa36d8bcab0562c72dc))
* **main:** release 1.0.2 ([4672000](https://github.com/AndrewM-F/code-foundry/commit/46720001f9b783974a3edfc7a5c7abd43abdfa7c))
* **main:** release 1.0.3 ([e9e7d4a](https://github.com/AndrewM-F/code-foundry/commit/e9e7d4af1e075f7d16b9695ccab39866a780d084))
* **main:** release 1.0.4 ([fdf0629](https://github.com/AndrewM-F/code-foundry/commit/fdf062988bb01977b4f4ed772ee5d36a894663b3))
* **main:** release 1.0.5 ([a954235](https://github.com/AndrewM-F/code-foundry/commit/a954235bc8c0cb10f4f0231e68a2fbccf6c09404))
* **main:** release 1.0.6 ([ce01c32](https://github.com/AndrewM-F/code-foundry/commit/ce01c328085165439aa2ef0d223b88d86199a112))
* **main:** release 1.1.0 ([21febb2](https://github.com/AndrewM-F/code-foundry/commit/21febb2265f358f1af41685a0692f136ec0c50b4))
* **main:** release 1.1.1 ([2e6d2cd](https://github.com/AndrewM-F/code-foundry/commit/2e6d2cdcb8c06f8d505cefa3238f5fd808651a1f))
* **main:** release 1.10.0 ([#532](https://github.com/AndrewM-F/code-foundry/issues/532)) ([a7c07ec](https://github.com/AndrewM-F/code-foundry/commit/a7c07ecda9238b09b3c3fde78da7aa9779935ce5))
* **main:** release 1.10.1 ([#541](https://github.com/AndrewM-F/code-foundry/issues/541)) ([ad64a88](https://github.com/AndrewM-F/code-foundry/commit/ad64a880f565b6e41f8f72178ad4dab3f19234ee))
* **main:** release 1.11.0 ([#542](https://github.com/AndrewM-F/code-foundry/issues/542)) ([335963d](https://github.com/AndrewM-F/code-foundry/commit/335963d33a5deec9ee25cd1aab27a89dbda25957))
* **main:** release 1.12.0 ([#543](https://github.com/AndrewM-F/code-foundry/issues/543)) ([ea86e62](https://github.com/AndrewM-F/code-foundry/commit/ea86e62085261e89b684801e522c5e7870483129))
* **main:** release 1.13.0 ([#546](https://github.com/AndrewM-F/code-foundry/issues/546)) ([d18b823](https://github.com/AndrewM-F/code-foundry/commit/d18b8236670f9b93649030a7e23150447029ef82))
* **main:** release 1.14.0 ([#550](https://github.com/AndrewM-F/code-foundry/issues/550)) ([93eb09e](https://github.com/AndrewM-F/code-foundry/commit/93eb09ec84302971280df991374f15d0fe86e47a))
* **main:** release 1.15.0 ([#551](https://github.com/AndrewM-F/code-foundry/issues/551)) ([ccb7942](https://github.com/AndrewM-F/code-foundry/commit/ccb7942cfe78dd664b26ed3c161c0721660ba60e))
* **main:** release 1.16.0 ([#552](https://github.com/AndrewM-F/code-foundry/issues/552)) ([af12167](https://github.com/AndrewM-F/code-foundry/commit/af12167c838cc065094d7c12458b31f682fd175f))
* **main:** release 1.17.0 ([#553](https://github.com/AndrewM-F/code-foundry/issues/553)) ([2ed63df](https://github.com/AndrewM-F/code-foundry/commit/2ed63dff786d5ba4c0fbb4b9bd0b2c641ad1a3b1))
* **main:** release 1.18.0 ([#554](https://github.com/AndrewM-F/code-foundry/issues/554)) ([381eee5](https://github.com/AndrewM-F/code-foundry/commit/381eee50599b78baf47f4f1c6b96e88cc6d0c331))
* **main:** release 1.19.0 ([#555](https://github.com/AndrewM-F/code-foundry/issues/555)) ([8a572fa](https://github.com/AndrewM-F/code-foundry/commit/8a572fa8162ef6287b9ee355ff355b96649ae474))
* **main:** release 1.2.0 ([01c73bf](https://github.com/AndrewM-F/code-foundry/commit/01c73bf3d02779f2db245bf70658fb449ff85711))
* **main:** release 1.2.1 ([fa86e25](https://github.com/AndrewM-F/code-foundry/commit/fa86e25c406c06390e4d435ca10fc67bb55bdef1))
* **main:** release 1.20.0 ([#559](https://github.com/AndrewM-F/code-foundry/issues/559)) ([7724ecb](https://github.com/AndrewM-F/code-foundry/commit/7724ecb574615804d7ac09b921dd05d6e309b966))
* **main:** release 1.20.1 ([#560](https://github.com/AndrewM-F/code-foundry/issues/560)) ([0ee6c36](https://github.com/AndrewM-F/code-foundry/commit/0ee6c36df65c9e1e9d66432353f415a3b2b3639f))
* **main:** release 1.20.2 ([#561](https://github.com/AndrewM-F/code-foundry/issues/561)) ([41dcf5b](https://github.com/AndrewM-F/code-foundry/commit/41dcf5bb52cd02b5f08d1ef84ef6cd69b56b3fea))
* **main:** release 1.21.0 ([#563](https://github.com/AndrewM-F/code-foundry/issues/563)) ([1bc4868](https://github.com/AndrewM-F/code-foundry/commit/1bc48685a8725f17550df4e2756867211240588a))
* **main:** release 1.21.1 ([#566](https://github.com/AndrewM-F/code-foundry/issues/566)) ([a97394d](https://github.com/AndrewM-F/code-foundry/commit/a97394d83f5761f121e36d20dfca73f0a427d86d))
* **main:** release 1.21.2 ([#569](https://github.com/AndrewM-F/code-foundry/issues/569)) ([fe0620b](https://github.com/AndrewM-F/code-foundry/commit/fe0620bc8779f6157470c57df56cdc97d7636e0b))
* **main:** release 1.21.3 ([#571](https://github.com/AndrewM-F/code-foundry/issues/571)) ([44c0dfc](https://github.com/AndrewM-F/code-foundry/commit/44c0dfc154dd71f665dda12b48b57f4729f02dec))
* **main:** release 1.22.0 ([#573](https://github.com/AndrewM-F/code-foundry/issues/573)) ([55ad8c6](https://github.com/AndrewM-F/code-foundry/commit/55ad8c60a32625b41b3e9a75177eb2b6518d62b1))
* **main:** release 1.22.1 ([#575](https://github.com/AndrewM-F/code-foundry/issues/575)) ([6e11ef5](https://github.com/AndrewM-F/code-foundry/commit/6e11ef56dc189a5d34812ab8ff978a32fc3a0a50))
* **main:** release 1.23.0 ([#577](https://github.com/AndrewM-F/code-foundry/issues/577)) ([4212c5c](https://github.com/AndrewM-F/code-foundry/commit/4212c5c6e1f4c5380bfa4eec3db6ef784551d8c5))
* **main:** release 1.24.0 ([#581](https://github.com/AndrewM-F/code-foundry/issues/581)) ([60ebabc](https://github.com/AndrewM-F/code-foundry/commit/60ebabc22424bb1cae9e8275d2cdbcd2515cf5b2))
* **main:** release 1.25.0 ([#582](https://github.com/AndrewM-F/code-foundry/issues/582)) ([313158b](https://github.com/AndrewM-F/code-foundry/commit/313158b4091770dd427282304eb079a8a183e066))
* **main:** release 1.25.1 ([#584](https://github.com/AndrewM-F/code-foundry/issues/584)) ([772c40b](https://github.com/AndrewM-F/code-foundry/commit/772c40b7d4f3f0bedfc39196eac7c3f08d6a3213))
* **main:** release 1.25.2 ([#586](https://github.com/AndrewM-F/code-foundry/issues/586)) ([f0eeb3d](https://github.com/AndrewM-F/code-foundry/commit/f0eeb3d936aa31547c3bd1929a2e882824c37e19))
* **main:** release 1.25.3 ([#588](https://github.com/AndrewM-F/code-foundry/issues/588)) ([a2685db](https://github.com/AndrewM-F/code-foundry/commit/a2685db2953b0104ad2049813e1125e6e0251e0b))
* **main:** release 1.26.0 ([#592](https://github.com/AndrewM-F/code-foundry/issues/592)) ([a2588eb](https://github.com/AndrewM-F/code-foundry/commit/a2588eb9c3e2bfb504f055c104618dbcb0095906))
* **main:** release 1.27.0 ([#593](https://github.com/AndrewM-F/code-foundry/issues/593)) ([d3df83b](https://github.com/AndrewM-F/code-foundry/commit/d3df83b03bf2d002d8a8142252fcab9b1f4df014))
* **main:** release 1.28.0 ([#594](https://github.com/AndrewM-F/code-foundry/issues/594)) ([a325698](https://github.com/AndrewM-F/code-foundry/commit/a325698184598319647c32d3384c018eb132682b))
* **main:** release 1.28.1 ([#596](https://github.com/AndrewM-F/code-foundry/issues/596)) ([7e2e7b7](https://github.com/AndrewM-F/code-foundry/commit/7e2e7b724aa2cb7cef7e5116528d0db3f76c5387))
* **main:** release 1.28.10 ([#615](https://github.com/AndrewM-F/code-foundry/issues/615)) ([427eb67](https://github.com/AndrewM-F/code-foundry/commit/427eb67b3958c0214ed19436f6981b0b71226a84))
* **main:** release 1.28.11 ([#617](https://github.com/AndrewM-F/code-foundry/issues/617)) ([e406d8a](https://github.com/AndrewM-F/code-foundry/commit/e406d8a97c9ff35fa18ecc56d07cbece2ca61ac9))
* **main:** release 1.28.12 ([#619](https://github.com/AndrewM-F/code-foundry/issues/619)) ([17ab57e](https://github.com/AndrewM-F/code-foundry/commit/17ab57e9df5d56f785265662a4dc40dab701821f))
* **main:** release 1.28.13 ([#622](https://github.com/AndrewM-F/code-foundry/issues/622)) ([f605942](https://github.com/AndrewM-F/code-foundry/commit/f60594248e4037e722cc31887477678027cbd3f7))
* **main:** release 1.28.14 ([#623](https://github.com/AndrewM-F/code-foundry/issues/623)) ([960d94b](https://github.com/AndrewM-F/code-foundry/commit/960d94b69a2b699708ddf2b60ef689300fad79a5))
* **main:** release 1.28.15 ([#625](https://github.com/AndrewM-F/code-foundry/issues/625)) ([2e4b801](https://github.com/AndrewM-F/code-foundry/commit/2e4b8010181bbdc6e8885d3766e8690546721d39))
* **main:** release 1.28.2 ([#598](https://github.com/AndrewM-F/code-foundry/issues/598)) ([9f95f1c](https://github.com/AndrewM-F/code-foundry/commit/9f95f1c09625a52aa805b5a8b953744cd50b7635))
* **main:** release 1.28.3 ([#600](https://github.com/AndrewM-F/code-foundry/issues/600)) ([6fdb715](https://github.com/AndrewM-F/code-foundry/commit/6fdb71504d201dccd4b8766f6522894b6c390857))
* **main:** release 1.28.4 ([#602](https://github.com/AndrewM-F/code-foundry/issues/602)) ([e098bab](https://github.com/AndrewM-F/code-foundry/commit/e098babda5b9b617fecedb7ddafa5b385621a326))
* **main:** release 1.28.5 ([#604](https://github.com/AndrewM-F/code-foundry/issues/604)) ([5da2766](https://github.com/AndrewM-F/code-foundry/commit/5da2766b9244bb16c135f62fa53b12f6ec9f040c))
* **main:** release 1.28.6 ([#606](https://github.com/AndrewM-F/code-foundry/issues/606)) ([8883ff1](https://github.com/AndrewM-F/code-foundry/commit/8883ff11022a7686c67d7a72b683c9a149e39b17))
* **main:** release 1.28.7 ([#608](https://github.com/AndrewM-F/code-foundry/issues/608)) ([34824d5](https://github.com/AndrewM-F/code-foundry/commit/34824d5074d134532bbb467cd1de9fca4d517b84))
* **main:** release 1.28.8 ([#611](https://github.com/AndrewM-F/code-foundry/issues/611)) ([0089ccf](https://github.com/AndrewM-F/code-foundry/commit/0089ccf7559af4065ec66e11a838b92f46f54b73))
* **main:** release 1.28.9 ([#614](https://github.com/AndrewM-F/code-foundry/issues/614)) ([837f1a4](https://github.com/AndrewM-F/code-foundry/commit/837f1a4275ab1606ee1b4ac8cc520a46e37c4ca2))
* **main:** release 1.29.0 ([#627](https://github.com/AndrewM-F/code-foundry/issues/627)) ([f601a21](https://github.com/AndrewM-F/code-foundry/commit/f601a21db86ebc12829c45f92f6ec5c662b40604))
* **main:** release 1.29.1 ([#629](https://github.com/AndrewM-F/code-foundry/issues/629)) ([3171886](https://github.com/AndrewM-F/code-foundry/commit/3171886a345a1fc044f047450fa662f413c43f4f))
* **main:** release 1.3.0 ([37af8c2](https://github.com/AndrewM-F/code-foundry/commit/37af8c2eb2b1136d038faf9d76dc1312c65ad44a))
* **main:** release 1.3.1 ([b482369](https://github.com/AndrewM-F/code-foundry/commit/b482369b1d5364c056d984dd518aaef42f761de4))
* **main:** release 1.3.2 ([84d8cfe](https://github.com/AndrewM-F/code-foundry/commit/84d8cfe17fd8d4c7b41235f37b06a91f86956eae))
* **main:** release 1.30.0 ([#632](https://github.com/AndrewM-F/code-foundry/issues/632)) ([4c03dae](https://github.com/AndrewM-F/code-foundry/commit/4c03daec5cc1a4327084fbda35e641d59da33e89))
* **main:** release 1.30.1 ([#633](https://github.com/AndrewM-F/code-foundry/issues/633)) ([39a6c2e](https://github.com/AndrewM-F/code-foundry/commit/39a6c2e3d3cfa389314f2fac30482faa7380a878))
* **main:** release 1.30.2 ([#635](https://github.com/AndrewM-F/code-foundry/issues/635)) ([f943e22](https://github.com/AndrewM-F/code-foundry/commit/f943e22d97b2b002ea3bfce26ada86ba92d36206))
* **main:** release 1.31.0 ([#637](https://github.com/AndrewM-F/code-foundry/issues/637)) ([bc4c526](https://github.com/AndrewM-F/code-foundry/commit/bc4c526cafed611262323a23a322eae0572bb8a4))
* **main:** release 1.32.0 ([#639](https://github.com/AndrewM-F/code-foundry/issues/639)) ([8d4b1de](https://github.com/AndrewM-F/code-foundry/commit/8d4b1ded29c2e7b8741661a7181fedb06d09fb80))
* **main:** release 1.33.0 ([#641](https://github.com/AndrewM-F/code-foundry/issues/641)) ([8acc875](https://github.com/AndrewM-F/code-foundry/commit/8acc8758ffbc7effc5ba53a9298b4241341a8670))
* **main:** release 1.33.1 ([#644](https://github.com/AndrewM-F/code-foundry/issues/644)) ([e700804](https://github.com/AndrewM-F/code-foundry/commit/e700804bcca74312e9102531089dc7774ac6c0c0))
* **main:** release 1.33.2 ([#647](https://github.com/AndrewM-F/code-foundry/issues/647)) ([f13dc87](https://github.com/AndrewM-F/code-foundry/commit/f13dc87982d5423414a3c11d94830358bd5f890a))
* **main:** release 1.33.3 ([#650](https://github.com/AndrewM-F/code-foundry/issues/650)) ([d0834f1](https://github.com/AndrewM-F/code-foundry/commit/d0834f1f354bfca98aa1bd3fca62fc24114ce3b7))
* **main:** release 1.34.0 ([#652](https://github.com/AndrewM-F/code-foundry/issues/652)) ([c0b1c93](https://github.com/AndrewM-F/code-foundry/commit/c0b1c9300e2e5047a5ad512aa081f75018e874fb))
* **main:** release 1.35.0 ([#656](https://github.com/AndrewM-F/code-foundry/issues/656)) ([c8aebd7](https://github.com/AndrewM-F/code-foundry/commit/c8aebd77aab88dff6d648ca26d660fdf505fae33))
* **main:** release 1.36.0 ([#659](https://github.com/AndrewM-F/code-foundry/issues/659)) ([8e1c893](https://github.com/AndrewM-F/code-foundry/commit/8e1c8933fecbd55504d8bf694561d2a11e9f2f77))
* **main:** release 1.36.1 ([#661](https://github.com/AndrewM-F/code-foundry/issues/661)) ([6b3f0a9](https://github.com/AndrewM-F/code-foundry/commit/6b3f0a91d3e24bf102231456cb5419555b43748e))
* **main:** release 1.36.2 ([#663](https://github.com/AndrewM-F/code-foundry/issues/663)) ([25f7c87](https://github.com/AndrewM-F/code-foundry/commit/25f7c87b8ee41d54f0d41fcc50c696cd62177170))
* **main:** release 1.36.3 ([#665](https://github.com/AndrewM-F/code-foundry/issues/665)) ([d932af0](https://github.com/AndrewM-F/code-foundry/commit/d932af0dca9367d502913ea2e1ed453ddf9663a1))
* **main:** release 1.36.4 ([#666](https://github.com/AndrewM-F/code-foundry/issues/666)) ([4bbdebf](https://github.com/AndrewM-F/code-foundry/commit/4bbdebfa6588300ec74a404474ec284e3114d830))
* **main:** release 1.37.0 ([#669](https://github.com/AndrewM-F/code-foundry/issues/669)) ([847b666](https://github.com/AndrewM-F/code-foundry/commit/847b666b2a095c5c627b5bf236cf1f1f791356e6))
* **main:** release 1.37.1 ([#671](https://github.com/AndrewM-F/code-foundry/issues/671)) ([34e2c3c](https://github.com/AndrewM-F/code-foundry/commit/34e2c3cc89d4ae32c1e30fb94f72d7b78dd3942e))
* **main:** release 1.37.2 ([#673](https://github.com/AndrewM-F/code-foundry/issues/673)) ([836bc05](https://github.com/AndrewM-F/code-foundry/commit/836bc05be27153704eb5177e08cac118ccf2c8a8))
* **main:** release 1.37.3 ([#675](https://github.com/AndrewM-F/code-foundry/issues/675)) ([59446cb](https://github.com/AndrewM-F/code-foundry/commit/59446cb79d34babf311165e14e20faeb89488d78))
* **main:** release 1.38.0 ([#677](https://github.com/AndrewM-F/code-foundry/issues/677)) ([4e26060](https://github.com/AndrewM-F/code-foundry/commit/4e26060f888cc674cb9ea94779d2a3fc41f37836))
* **main:** release 1.38.1 ([#679](https://github.com/AndrewM-F/code-foundry/issues/679)) ([fa94e52](https://github.com/AndrewM-F/code-foundry/commit/fa94e5203fd4a648c0e470dd2e4d9e7612d34f67))
* **main:** release 1.39.0 ([#685](https://github.com/AndrewM-F/code-foundry/issues/685)) ([6c789d0](https://github.com/AndrewM-F/code-foundry/commit/6c789d0f6f6fdf6d2022e813abfab5cce2031392))
* **main:** release 1.39.1 ([#686](https://github.com/AndrewM-F/code-foundry/issues/686)) ([cea2fc4](https://github.com/AndrewM-F/code-foundry/commit/cea2fc42db691d29e72fdbf923780dc6c46f16b8))
* **main:** release 1.39.2 ([#687](https://github.com/AndrewM-F/code-foundry/issues/687)) ([4565ee2](https://github.com/AndrewM-F/code-foundry/commit/4565ee23d942c942ace445a2278e9d8cb1eb3152))
* **main:** release 1.39.3 ([#689](https://github.com/AndrewM-F/code-foundry/issues/689)) ([4480cfe](https://github.com/AndrewM-F/code-foundry/commit/4480cfe6c59bd8005a19c3016fa3932d2a91ecfa))
* **main:** release 1.4.0 ([da5f0e8](https://github.com/AndrewM-F/code-foundry/commit/da5f0e8898d6968043c1f2c9e9f2b443aa24ce3d))
* **main:** release 1.4.1 ([23ec58a](https://github.com/AndrewM-F/code-foundry/commit/23ec58a9595a6095ad5506356030a13792d3843c))
* **main:** release 1.40.0 ([#693](https://github.com/AndrewM-F/code-foundry/issues/693)) ([445b897](https://github.com/AndrewM-F/code-foundry/commit/445b8972fd9182e016a57cc0d539fa060b0f9109))
* **main:** release 1.41.0 ([#695](https://github.com/AndrewM-F/code-foundry/issues/695)) ([d68fdfc](https://github.com/AndrewM-F/code-foundry/commit/d68fdfc6737b99b629510f900368bcc251fd152c))
* **main:** release 1.42.0 ([#698](https://github.com/AndrewM-F/code-foundry/issues/698)) ([2584b69](https://github.com/AndrewM-F/code-foundry/commit/2584b69cbb4c623a96284556d29bdc5bc402c98b))
* **main:** release 1.43.0 ([#701](https://github.com/AndrewM-F/code-foundry/issues/701)) ([c67c7ea](https://github.com/AndrewM-F/code-foundry/commit/c67c7ea8c0d05afa46dcea4dc395170baf7ce9b1))
* **main:** release 1.43.1 ([#704](https://github.com/AndrewM-F/code-foundry/issues/704)) ([ecd9120](https://github.com/AndrewM-F/code-foundry/commit/ecd912070eaf52784ef2adf8f75ff7f588d51c76))
* **main:** release 1.43.2 ([#706](https://github.com/AndrewM-F/code-foundry/issues/706)) ([927f31f](https://github.com/AndrewM-F/code-foundry/commit/927f31fcd301951834e9bc6116e56739c236eabe))
* **main:** release 1.44.0 ([#707](https://github.com/AndrewM-F/code-foundry/issues/707)) ([a6b9c40](https://github.com/AndrewM-F/code-foundry/commit/a6b9c4058ffb7fc7caf08f23acbd49cb57d27bff))
* **main:** release 1.44.1 ([#709](https://github.com/AndrewM-F/code-foundry/issues/709)) ([302cffd](https://github.com/AndrewM-F/code-foundry/commit/302cffd5346b1ada414b96657fdbcbbe7653598b))
* **main:** release 1.44.10 ([#728](https://github.com/AndrewM-F/code-foundry/issues/728)) ([867978a](https://github.com/AndrewM-F/code-foundry/commit/867978a266cc84f9d8d596d7628790994ca40fb0))
* **main:** release 1.44.11 ([#730](https://github.com/AndrewM-F/code-foundry/issues/730)) ([18f7616](https://github.com/AndrewM-F/code-foundry/commit/18f76163f4d3830633c5f3379287314fef8bcc93))
* **main:** release 1.44.2 ([#711](https://github.com/AndrewM-F/code-foundry/issues/711)) ([19f1ddf](https://github.com/AndrewM-F/code-foundry/commit/19f1ddf60de3bc8bafaa75e62dc1d4f6291f1f2c))
* **main:** release 1.44.3 ([#713](https://github.com/AndrewM-F/code-foundry/issues/713)) ([5cf576a](https://github.com/AndrewM-F/code-foundry/commit/5cf576a81f1022bcc09cd4e88d404f9bdda61b40))
* **main:** release 1.44.4 ([#715](https://github.com/AndrewM-F/code-foundry/issues/715)) ([51eb273](https://github.com/AndrewM-F/code-foundry/commit/51eb2734413154c3a6bb0f2b12ab0f602f6d0326))
* **main:** release 1.44.5 ([#717](https://github.com/AndrewM-F/code-foundry/issues/717)) ([130713c](https://github.com/AndrewM-F/code-foundry/commit/130713cded43eea30fbcc7f21e26ce41634b501f))
* **main:** release 1.44.6 ([#719](https://github.com/AndrewM-F/code-foundry/issues/719)) ([ba0ab68](https://github.com/AndrewM-F/code-foundry/commit/ba0ab6809008bfd50b5d9723a5ae44b3b6fdaecc))
* **main:** release 1.44.7 ([#721](https://github.com/AndrewM-F/code-foundry/issues/721)) ([c5ffeaf](https://github.com/AndrewM-F/code-foundry/commit/c5ffeafd932c040ab21ad5c9975b56af6c7b269d))
* **main:** release 1.44.8 ([#723](https://github.com/AndrewM-F/code-foundry/issues/723)) ([4d27ef2](https://github.com/AndrewM-F/code-foundry/commit/4d27ef2c99cabca1cf0156f1506814c912219a6f))
* **main:** release 1.44.9 ([#726](https://github.com/AndrewM-F/code-foundry/issues/726)) ([2480f0e](https://github.com/AndrewM-F/code-foundry/commit/2480f0e7ed00db6540e4cd08939be51ce2a93499))
* **main:** release 1.45.0 ([#732](https://github.com/AndrewM-F/code-foundry/issues/732)) ([d65be87](https://github.com/AndrewM-F/code-foundry/commit/d65be874c5170f152b6499798ec24fb7dd87d255))
* **main:** release 1.45.1 ([#734](https://github.com/AndrewM-F/code-foundry/issues/734)) ([519388f](https://github.com/AndrewM-F/code-foundry/commit/519388fb61e62abf80488e906235efaa70b9a051))
* **main:** release 1.45.2 ([#736](https://github.com/AndrewM-F/code-foundry/issues/736)) ([41d5eeb](https://github.com/AndrewM-F/code-foundry/commit/41d5eebcb6541e1fa43faeda08b1c3900402aced))
* **main:** release 1.46.0 ([#739](https://github.com/AndrewM-F/code-foundry/issues/739)) ([04080f0](https://github.com/AndrewM-F/code-foundry/commit/04080f05428256c905f4d1c09c29d6b518998693))
* **main:** release 1.46.1 ([#741](https://github.com/AndrewM-F/code-foundry/issues/741)) ([d5b4cb6](https://github.com/AndrewM-F/code-foundry/commit/d5b4cb68d34923d55f5b816d81cddee704f6f485))
* **main:** release 1.46.2 ([#743](https://github.com/AndrewM-F/code-foundry/issues/743)) ([0743d40](https://github.com/AndrewM-F/code-foundry/commit/0743d409b63f0d2bd3c08626787ae4fbfac9b119))
* **main:** release 1.46.3 ([#745](https://github.com/AndrewM-F/code-foundry/issues/745)) ([5c7474e](https://github.com/AndrewM-F/code-foundry/commit/5c7474ed7a876bb1f176d2c71c28ecb799ce8318))
* **main:** release 1.46.4 ([#746](https://github.com/AndrewM-F/code-foundry/issues/746)) ([7704769](https://github.com/AndrewM-F/code-foundry/commit/77047696e858149316eecd96fc2865e7f0a50f16))
* **main:** release 1.46.5 ([#750](https://github.com/AndrewM-F/code-foundry/issues/750)) ([17773e1](https://github.com/AndrewM-F/code-foundry/commit/17773e1b767f66f4e7f3d4dede4aa2a3aacfee80))
* **main:** release 1.46.6 ([#751](https://github.com/AndrewM-F/code-foundry/issues/751)) ([1b8aae9](https://github.com/AndrewM-F/code-foundry/commit/1b8aae9812e5c673540a6a3aa8ad567d2df2fcb7))
* **main:** release 1.47.0 ([#752](https://github.com/AndrewM-F/code-foundry/issues/752)) ([c09116d](https://github.com/AndrewM-F/code-foundry/commit/c09116dc934fd1e44968c2e571e9a7478aaa1f3e))
* **main:** release 1.47.1 ([#754](https://github.com/AndrewM-F/code-foundry/issues/754)) ([b0d4660](https://github.com/AndrewM-F/code-foundry/commit/b0d4660d8a95ab9b6eaf6a880735792698afd407))
* **main:** release 1.47.2 ([#756](https://github.com/AndrewM-F/code-foundry/issues/756)) ([e83e7d5](https://github.com/AndrewM-F/code-foundry/commit/e83e7d54fa56354a15bc3adf3688a322fc3c1293))
* **main:** release 1.47.3 ([#758](https://github.com/AndrewM-F/code-foundry/issues/758)) ([6fe3e1a](https://github.com/AndrewM-F/code-foundry/commit/6fe3e1ab682f9989097a403d738775c2e1eeb55c))
* **main:** release 1.47.4 ([#761](https://github.com/AndrewM-F/code-foundry/issues/761)) ([a94275b](https://github.com/AndrewM-F/code-foundry/commit/a94275b8c877cee6b48423e9449019858a7d17ff))
* **main:** release 1.47.5 ([#762](https://github.com/AndrewM-F/code-foundry/issues/762)) ([2076d42](https://github.com/AndrewM-F/code-foundry/commit/2076d42d9f17927dfdacf2549efdfbe6bf75807e))
* **main:** release 1.48.0 ([#764](https://github.com/AndrewM-F/code-foundry/issues/764)) ([17506c9](https://github.com/AndrewM-F/code-foundry/commit/17506c9effce18797716090375d957b4f80bd5fb))
* **main:** release 1.48.1 ([#766](https://github.com/AndrewM-F/code-foundry/issues/766)) ([76cea74](https://github.com/AndrewM-F/code-foundry/commit/76cea74d165db1adaa45be0a828620b771d3000d))
* **main:** release 1.48.2 ([#768](https://github.com/AndrewM-F/code-foundry/issues/768)) ([390ccf7](https://github.com/AndrewM-F/code-foundry/commit/390ccf77790480d6f0286e0a18654a29993452a1))
* **main:** release 1.48.3 ([#770](https://github.com/AndrewM-F/code-foundry/issues/770)) ([695a993](https://github.com/AndrewM-F/code-foundry/commit/695a993ea70bf562a1cf0070af2a3dacefd87912))
* **main:** release 1.48.4 ([#772](https://github.com/AndrewM-F/code-foundry/issues/772)) ([39430d8](https://github.com/AndrewM-F/code-foundry/commit/39430d8617b15edeb9552959b8042623a7362975))
* **main:** release 1.48.5 ([#774](https://github.com/AndrewM-F/code-foundry/issues/774)) ([d669f8a](https://github.com/AndrewM-F/code-foundry/commit/d669f8afc1ac247f377422942e113ccf7b382945))
* **main:** release 1.48.6 ([#776](https://github.com/AndrewM-F/code-foundry/issues/776)) ([5b556b6](https://github.com/AndrewM-F/code-foundry/commit/5b556b60dd2942340fa7088803cbb0530196e242))
* **main:** release 1.48.7 ([#778](https://github.com/AndrewM-F/code-foundry/issues/778)) ([a8089e3](https://github.com/AndrewM-F/code-foundry/commit/a8089e3674d6a71b5e0c53eefe6ac0ef9fa8ac8b))
* **main:** release 1.48.8 ([#780](https://github.com/AndrewM-F/code-foundry/issues/780)) ([e152285](https://github.com/AndrewM-F/code-foundry/commit/e152285303da216b4978e42801479f6943fba032))
* **main:** release 1.48.9 ([#782](https://github.com/AndrewM-F/code-foundry/issues/782)) ([946d20a](https://github.com/AndrewM-F/code-foundry/commit/946d20a1c329fc2e8268d5e7331546da311e1f5b))
* **main:** release 1.49.0 ([#784](https://github.com/AndrewM-F/code-foundry/issues/784)) ([bad446d](https://github.com/AndrewM-F/code-foundry/commit/bad446d380e3349260bf81f2ea495068474b1491))
* **main:** release 1.49.1 ([#786](https://github.com/AndrewM-F/code-foundry/issues/786)) ([ebda019](https://github.com/AndrewM-F/code-foundry/commit/ebda01942cd2a1659c3e31e711da21df064e8c79))
* **main:** release 1.49.2 ([#788](https://github.com/AndrewM-F/code-foundry/issues/788)) ([637d105](https://github.com/AndrewM-F/code-foundry/commit/637d105f1569c80289aff037c9ce341460557445))
* **main:** release 1.49.3 ([#790](https://github.com/AndrewM-F/code-foundry/issues/790)) ([20dc2b2](https://github.com/AndrewM-F/code-foundry/commit/20dc2b255b5d80eb00666c4f30e555bd1bd5ecb0))
* **main:** release 1.5.0 ([2a228ad](https://github.com/AndrewM-F/code-foundry/commit/2a228ad8201ab62a06fcb34504d35ac0ba974a02))
* **main:** release 1.5.1 ([3135a7a](https://github.com/AndrewM-F/code-foundry/commit/3135a7a597fe4aa8ad53cf0823804c265e01ebfe))
* **main:** release 1.5.2 ([0b2beae](https://github.com/AndrewM-F/code-foundry/commit/0b2beaebc8c3e028db1060dbfee1169034d97dbe))
* **main:** release 1.5.3 ([a430f36](https://github.com/AndrewM-F/code-foundry/commit/a430f3601314d4c97fbeae7d866a8c1ca44bf260))
* **main:** release 1.5.4 ([8e7e1a1](https://github.com/AndrewM-F/code-foundry/commit/8e7e1a1e4282456ae2f33698744b727a54cac012))
* **main:** release 1.50.0 ([#792](https://github.com/AndrewM-F/code-foundry/issues/792)) ([6d372c4](https://github.com/AndrewM-F/code-foundry/commit/6d372c4214d624a4d69e7f274dd8704e6c98ee69))
* **main:** release 1.50.1 ([#794](https://github.com/AndrewM-F/code-foundry/issues/794)) ([52ffa00](https://github.com/AndrewM-F/code-foundry/commit/52ffa008a60c2b9f1314efbcbf6a1d1865335337))
* **main:** release 1.51.0 ([#796](https://github.com/AndrewM-F/code-foundry/issues/796)) ([b18107e](https://github.com/AndrewM-F/code-foundry/commit/b18107e9ca5200981481666fc08eaac516f66151))
* **main:** release 1.51.1 ([#798](https://github.com/AndrewM-F/code-foundry/issues/798)) ([29bf1d4](https://github.com/AndrewM-F/code-foundry/commit/29bf1d4bfd1fded716e11f8f930daae5e83f87bd))
* **main:** release 1.52.0 ([#803](https://github.com/AndrewM-F/code-foundry/issues/803)) ([e40f65b](https://github.com/AndrewM-F/code-foundry/commit/e40f65bd3f5282895ebc27b36dfa93e535a20ad9))
* **main:** release 1.52.1 ([#804](https://github.com/AndrewM-F/code-foundry/issues/804)) ([23dbf94](https://github.com/AndrewM-F/code-foundry/commit/23dbf94adef524658a43727b41fffc6966855da0))
* **main:** release 1.52.2 ([#806](https://github.com/AndrewM-F/code-foundry/issues/806)) ([4e777d5](https://github.com/AndrewM-F/code-foundry/commit/4e777d5de74f8b2777fe1505d1b67d8f9cce9524))
* **main:** release 1.52.3 ([#807](https://github.com/AndrewM-F/code-foundry/issues/807)) ([46dd960](https://github.com/AndrewM-F/code-foundry/commit/46dd9600790ea2951fd79a11c5b0a4496452622a))
* **main:** release 1.52.4 ([#809](https://github.com/AndrewM-F/code-foundry/issues/809)) ([fb701df](https://github.com/AndrewM-F/code-foundry/commit/fb701dfe5a07c4ab0a708f3e24e9eec72846e1c8))
* **main:** release 1.53.0 ([#812](https://github.com/AndrewM-F/code-foundry/issues/812)) ([aa4a344](https://github.com/AndrewM-F/code-foundry/commit/aa4a34486c98956d707d56d315d0df3763cea1ed))
* **main:** release 1.53.1 ([#814](https://github.com/AndrewM-F/code-foundry/issues/814)) ([5f5e6e4](https://github.com/AndrewM-F/code-foundry/commit/5f5e6e460fc48c3fa88250729f493b826117edf1))
* **main:** release 1.53.10 ([#834](https://github.com/AndrewM-F/code-foundry/issues/834)) ([a2b430f](https://github.com/AndrewM-F/code-foundry/commit/a2b430f81e4bccdbe0b6a02c7f1f505986b3f517))
* **main:** release 1.53.11 ([#835](https://github.com/AndrewM-F/code-foundry/issues/835)) ([5fa9772](https://github.com/AndrewM-F/code-foundry/commit/5fa9772d57115a905514e671c541e150181f93e1))
* **main:** release 1.53.12 ([#839](https://github.com/AndrewM-F/code-foundry/issues/839)) ([a454f88](https://github.com/AndrewM-F/code-foundry/commit/a454f8818ae7c2f0c857ca8741d5b4dd5b231698))
* **main:** release 1.53.2 ([#818](https://github.com/AndrewM-F/code-foundry/issues/818)) ([85b11c5](https://github.com/AndrewM-F/code-foundry/commit/85b11c5e83462f8fbe35d923330ab260b79c0c7a))
* **main:** release 1.53.3 ([#820](https://github.com/AndrewM-F/code-foundry/issues/820)) ([881ab72](https://github.com/AndrewM-F/code-foundry/commit/881ab723e0db55df43aa2eaaa0e5072e227e0201))
* **main:** release 1.53.4 ([#822](https://github.com/AndrewM-F/code-foundry/issues/822)) ([560e125](https://github.com/AndrewM-F/code-foundry/commit/560e125b405bdeba31a0ee3f6de841bb9c09d82d))
* **main:** release 1.53.5 ([#824](https://github.com/AndrewM-F/code-foundry/issues/824)) ([be1deac](https://github.com/AndrewM-F/code-foundry/commit/be1deac6d477af76bae87c2620a5e63a12179033))
* **main:** release 1.53.6 ([#826](https://github.com/AndrewM-F/code-foundry/issues/826)) ([8b62e89](https://github.com/AndrewM-F/code-foundry/commit/8b62e8923b30fb08c82fc3ba6bd7f20085b5be3f))
* **main:** release 1.53.7 ([#828](https://github.com/AndrewM-F/code-foundry/issues/828)) ([d5739e3](https://github.com/AndrewM-F/code-foundry/commit/d5739e36a0633199a214b1aab46b521efae870dc))
* **main:** release 1.53.8 ([#830](https://github.com/AndrewM-F/code-foundry/issues/830)) ([745e54b](https://github.com/AndrewM-F/code-foundry/commit/745e54b96397ee214b1e29045814c4a8115db56c))
* **main:** release 1.53.9 ([#832](https://github.com/AndrewM-F/code-foundry/issues/832)) ([7e2dd8d](https://github.com/AndrewM-F/code-foundry/commit/7e2dd8d2f20a8df98a05970b76fc72346ab7db95))
* **main:** release 1.54.0 ([#841](https://github.com/AndrewM-F/code-foundry/issues/841)) ([1c044b8](https://github.com/AndrewM-F/code-foundry/commit/1c044b8d0bb8bfccae75348bf33219e303ce40ae))
* **main:** release 1.54.1 ([#843](https://github.com/AndrewM-F/code-foundry/issues/843)) ([a15b3c1](https://github.com/AndrewM-F/code-foundry/commit/a15b3c1c722f8818ac3cc70f644b067dd2073dbc))
* **main:** release 1.6.0 ([5985a2e](https://github.com/AndrewM-F/code-foundry/commit/5985a2e44db339d7c95c0e862f2873e1188977c8))
* **main:** release 1.6.1 ([b2a6335](https://github.com/AndrewM-F/code-foundry/commit/b2a6335e1b9a9eb3952a65eb4f933fd5a7e03862))
* **main:** release 1.7.0 ([#498](https://github.com/AndrewM-F/code-foundry/issues/498)) ([05ee98f](https://github.com/AndrewM-F/code-foundry/commit/05ee98fb4c028d6a0c027dd2f459c19d575d42c3))
* **main:** release 1.8.0 ([#500](https://github.com/AndrewM-F/code-foundry/issues/500)) ([5119e85](https://github.com/AndrewM-F/code-foundry/commit/5119e856ff0c6f5808e439eefca543e54fa2eebd))
* **main:** release 1.9.0 ([#502](https://github.com/AndrewM-F/code-foundry/issues/502)) ([08b2887](https://github.com/AndrewM-F/code-foundry/commit/08b2887555b35685225cf7c020257763300b36b5))
* **main:** release 1.9.1 ([#504](https://github.com/AndrewM-F/code-foundry/issues/504)) ([39b8793](https://github.com/AndrewM-F/code-foundry/commit/39b8793e8fc4357787ac6f3fd43622de2777789a))
* **main:** release 1.9.10 ([#524](https://github.com/AndrewM-F/code-foundry/issues/524)) ([6ace253](https://github.com/AndrewM-F/code-foundry/commit/6ace253177040853e6a06872f89b5ea4fb797991))
* **main:** release 1.9.11 ([#526](https://github.com/AndrewM-F/code-foundry/issues/526)) ([c402607](https://github.com/AndrewM-F/code-foundry/commit/c40260768c63973f2438a9137ef250d442886b19))
* **main:** release 1.9.12 ([#528](https://github.com/AndrewM-F/code-foundry/issues/528)) ([1547065](https://github.com/AndrewM-F/code-foundry/commit/154706570a3b49d286333914a970200ca3a9bc0e))
* **main:** release 1.9.13 ([#531](https://github.com/AndrewM-F/code-foundry/issues/531)) ([1a284fc](https://github.com/AndrewM-F/code-foundry/commit/1a284fcb83914fcbdd9e74269512a255f6276fe3))
* **main:** release 1.9.2 ([#506](https://github.com/AndrewM-F/code-foundry/issues/506)) ([d57a1ce](https://github.com/AndrewM-F/code-foundry/commit/d57a1ce0fd53d3d9c2b9c64081e11893a7d461fc))
* **main:** release 1.9.3 ([#508](https://github.com/AndrewM-F/code-foundry/issues/508)) ([c3e2a99](https://github.com/AndrewM-F/code-foundry/commit/c3e2a99391a6db4874dd98a682c85961d20ce47c))
* **main:** release 1.9.4 ([#510](https://github.com/AndrewM-F/code-foundry/issues/510)) ([3c14973](https://github.com/AndrewM-F/code-foundry/commit/3c149730aa5d2587beda3603ecc977c8d3f42868))
* **main:** release 1.9.5 ([#512](https://github.com/AndrewM-F/code-foundry/issues/512)) ([f46143c](https://github.com/AndrewM-F/code-foundry/commit/f46143cd4bf5687705b10d909b8b86a196344a89))
* **main:** release 1.9.6 ([#514](https://github.com/AndrewM-F/code-foundry/issues/514)) ([cc34d08](https://github.com/AndrewM-F/code-foundry/commit/cc34d08d82eb6d7f4507e4179ab7176a24cbf8e6))
* **main:** release 1.9.7 ([#516](https://github.com/AndrewM-F/code-foundry/issues/516)) ([0aa0ac4](https://github.com/AndrewM-F/code-foundry/commit/0aa0ac4f11f7e4f69ab7369489dd74d09aa3d47e))
* **main:** release 1.9.8 ([#520](https://github.com/AndrewM-F/code-foundry/issues/520)) ([3a2e1f6](https://github.com/AndrewM-F/code-foundry/commit/3a2e1f61a60d1f639d174725d6461eea84a43561))
* **main:** release 1.9.9 ([#522](https://github.com/AndrewM-F/code-foundry/issues/522)) ([805dd77](https://github.com/AndrewM-F/code-foundry/commit/805dd77c8d629129cec7273dddfb4b61bc722442))
* **perf:** recalibrate the packed artifact budget ([#645](https://github.com/AndrewM-F/code-foundry/issues/645)) ([e789179](https://github.com/AndrewM-F/code-foundry/commit/e78917938243041ea0babc04adeeb8941b0d0f42))
* promote staging snapshot a2f7393bcba3 ([c434055](https://github.com/AndrewM-F/code-foundry/commit/c434055c36a57e5ed3c9318e92d3de42df3b8360))
* raise the packed artifact budget to 286 kB ([#657](https://github.com/AndrewM-F/code-foundry/issues/657)) ([0fb538c](https://github.com/AndrewM-F/code-foundry/commit/0fb538c9eb384c7605b0b3fc177a16a0a1d89865))
* register the adea-ai ui and themes consumers in the fleet manifest ([#680](https://github.com/AndrewM-F/code-foundry/issues/680)) ([1e41246](https://github.com/AndrewM-F/code-foundry/commit/1e412463aabdf93d6fe0c65e053f08fc89461e52))
* **scanners:** default opencode-security model to muse-spark-1.3 ([5560c02](https://github.com/AndrewM-F/code-foundry/commit/5560c02eb4892d40f8f0f1f42bbd3aff32633ded))
* **staging:** promote reconciled release-pr fixes ([86ada04](https://github.com/AndrewM-F/code-foundry/commit/86ada04e5ecb459845526bc4660bf9dad186f992))
* **staging:** promote release-pr REST fix ([e98eaab](https://github.com/AndrewM-F/code-foundry/commit/e98eaab38d95b125ae7e848609348e270f422a6f))
* toolchain-alignment ([#630](https://github.com/AndrewM-F/code-foundry/issues/630)) ([580d28a](https://github.com/AndrewM-F/code-foundry/commit/580d28ad70b6c1bfca4f7d87492127622d3f065b))
* **toolchain:** update to Bun 1.4 ([#410](https://github.com/AndrewM-F/code-foundry/issues/410)) ([090bd77](https://github.com/AndrewM-F/code-foundry/commit/090bd77df177db7e79933c585b35df7b59cca037))
* track the JavaScript Dependabot ecosystem as bun by default ([#648](https://github.com/AndrewM-F/code-foundry/issues/648)) ([3e4d9a1](https://github.com/AndrewM-F/code-foundry/commit/3e4d9a179d906efd26e65a7f83ead6c89ac08acc))

## [1.54.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.54.0...v1.54.1) (2026-11-09)


### Documentation

* **agents:** use GitButler and stop creating worktrees ([#842](https://github.com/0xPlayerOne/code-foundry/issues/842)) ([04d8091](https://github.com/0xPlayerOne/code-foundry/commit/04d809170403afa29a45d2cbc9679bf53e32f1d2))

## [1.54.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.12...v1.54.0) (2026-11-07)


### Features

* **runtime:** enforce an opt-in Build time ceiling ([#840](https://github.com/0xPlayerOne/code-foundry/issues/840)) ([a379a46](https://github.com/0xPlayerOne/code-foundry/commit/a379a46bc8e6749fff282ac9e45c77b714e72aa4))

## [1.53.12](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.11...v1.53.12) (2026-11-07)


### Bug Fixes

* complete runtime package declarations ([#838](https://github.com/0xPlayerOne/code-foundry/issues/838)) ([479a058](https://github.com/0xPlayerOne/code-foundry/commit/479a0587d5365977092844d2097d1286443c5ffd))

## [1.53.11](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.10...v1.53.11) (2026-10-31)


### Bug Fixes

* **draft-guard:** grant draft-mutation permission and respect same-second ready transitions ([913096f](https://github.com/0xPlayerOne/code-foundry/commit/913096f3b67144d7784325a3aa61dedcc0f17ee6))


### Tests

* tolerate runner contention in readiness fixtures ([#836](https://github.com/0xPlayerOne/code-foundry/issues/836)) ([26f2ec7](https://github.com/0xPlayerOne/code-foundry/commit/26f2ec77259cf883f15851351d37a955311f1b24))

## [1.53.10](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.9...v1.53.10) (2026-10-31)


### Bug Fixes

* **release:** stop version pull requests from closing referenced issues ([#833](https://github.com/0xPlayerOne/code-foundry/issues/833)) ([d912e46](https://github.com/0xPlayerOne/code-foundry/commit/d912e463275495fef91153d7b627e12f3a3ff2f4))

## [1.53.9](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.8...v1.53.9) (2026-10-31)


### Performance

* **codeql:** drop unchanged analyzers from the planned matrix ([#831](https://github.com/0xPlayerOne/code-foundry/issues/831)) ([35b891e](https://github.com/0xPlayerOne/code-foundry/commit/35b891e721ea2e5d2bd09ec44509b541120a3a64))

## [1.53.8](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.7...v1.53.8) (2026-10-31)


### Bug Fixes

* **release:** wait for the synchronize validation run before re-readying ([#829](https://github.com/0xPlayerOne/code-foundry/issues/829)) ([d0abbe2](https://github.com/0xPlayerOne/code-foundry/commit/d0abbe27349635bcc5bb63aafac3ff2e989f960f))

## [1.53.7](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.6...v1.53.7) (2026-10-31)


### Performance

* **validation:** fold Security Profile and CodeQL Detect into the plan job ([#827](https://github.com/0xPlayerOne/code-foundry/issues/827)) ([75ca83c](https://github.com/0xPlayerOne/code-foundry/commit/75ca83c042f01e23a1f3c62b26f92e1bc6641a80))

## [1.53.6](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.5...v1.53.6) (2026-10-31)


### Performance

* **validation:** skip lane jobs that have nothing to run ([#825](https://github.com/0xPlayerOne/code-foundry/issues/825)) ([4d04f62](https://github.com/0xPlayerOne/code-foundry/commit/4d04f627bfac572bc056b5a5f448b66c17500c00))

## [1.53.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.4...v1.53.5) (2026-10-31)


### Bug Fixes

* **codeql:** pass the event name so pull request change detection runs ([#823](https://github.com/0xPlayerOne/code-foundry/issues/823)) ([0d0044e](https://github.com/0xPlayerOne/code-foundry/commit/0d0044eca5dc5ec3457ea82892429d146ea1754d))

## [1.53.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.3...v1.53.4) (2026-10-30)


### Performance

* **ci:** run mixed unit runners concurrently ([#821](https://github.com/0xPlayerOne/code-foundry/issues/821)) ([dac0d93](https://github.com/0xPlayerOne/code-foundry/commit/dac0d9313cc2fc6309e0f55aa45274e3dbbff767))

## [1.53.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.2...v1.53.3) (2026-10-30)


### Bug Fixes

* save repository caches through an explicit save action ([#819](https://github.com/0xPlayerOne/code-foundry/issues/819)) ([a21f1d0](https://github.com/0xPlayerOne/code-foundry/commit/a21f1d0c153e14252bc784f301379029026121da))

## [1.53.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.1...v1.53.2) (2026-10-30)


### Bug Fixes

* support reviewed Playwright 1.64.1 UI receipts ([#817](https://github.com/0xPlayerOne/code-foundry/issues/817)) ([814bf68](https://github.com/0xPlayerOne/code-foundry/commit/814bf68818dcf2a80253e133895cbe3e539b5b7f))


### Maintenance

* add verified npm publication recovery ([#815](https://github.com/0xPlayerOne/code-foundry/issues/815)) ([5876361](https://github.com/0xPlayerOne/code-foundry/commit/58763616b3dc38d127680914eeef6151b3375b37))

## [1.53.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.53.0...v1.53.1) (2026-10-30)


### Bug Fixes

* allow isolated preview auth Hyperdrive build binding ([#813](https://github.com/0xPlayerOne/code-foundry/issues/813)) ([cc267fc](https://github.com/0xPlayerOne/code-foundry/commit/cc267fcb84c2828fb5c7090e0b494991ea90f249))

## [1.53.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.52.4...v1.53.0) (2026-10-30)


### Features

* document Adea UI workspace receipt reuse ([#811](https://github.com/0xPlayerOne/code-foundry/issues/811)) ([6d0322c](https://github.com/0xPlayerOne/code-foundry/commit/6d0322c619f82753ca1818523a7cb7fb6583934e))

## [1.52.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.52.3...v1.52.4) (2026-10-30)


### Bug Fixes

* recognize fixed test-and-pack receipt lifecycle ([#808](https://github.com/0xPlayerOne/code-foundry/issues/808)) ([8c8010c](https://github.com/0xPlayerOne/code-foundry/commit/8c8010cb926895d5a81289c696f82b855e30ad9f))

## [1.52.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.52.2...v1.52.3) (2026-10-30)


### Bug Fixes

* opt Code Foundry into source qualification receipts ([#805](https://github.com/0xPlayerOne/code-foundry/issues/805)) ([c7f7011](https://github.com/0xPlayerOne/code-foundry/commit/c7f70117b7d9d687d1116766114ba39028a4dc40))

## [1.52.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.52.1...v1.52.2) (2026-10-30)


### Bug Fixes

* retry transient release fallback reads safely ([#800](https://github.com/0xPlayerOne/code-foundry/issues/800)) ([c91e23b](https://github.com/0xPlayerOne/code-foundry/commit/c91e23bfaea9f107c8af9fa9bdf391308fa5ebf2))

## [1.52.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.52.0...v1.52.1) (2026-10-30)


### Bug Fixes

* restore source qualification receipt reuse ([#801](https://github.com/0xPlayerOne/code-foundry/issues/801)) ([989bdbf](https://github.com/0xPlayerOne/code-foundry/commit/989bdbfe5af6d2003ca97dde456d8c86fb92078c))

## [1.52.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.51.1...v1.52.0) (2026-10-30)


### Features

* scope Cloudflare build variables to build ([#802](https://github.com/0xPlayerOne/code-foundry/issues/802)) ([1f9a89f](https://github.com/0xPlayerOne/code-foundry/commit/1f9a89fa19a868732805a065fe90cc7609928a1e))


### Bug Fixes

* scope draft cancellation to its pull request ([#799](https://github.com/0xPlayerOne/code-foundry/issues/799)) ([ba42e81](https://github.com/0xPlayerOne/code-foundry/commit/ba42e811729e6ab8a82e2941abfdaab4f8544eed))

## [1.51.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.51.0...v1.51.1) (2026-10-29)


### Bug Fixes

* **ci:** run CodeQL on every main push ([#797](https://github.com/0xPlayerOne/code-foundry/issues/797)) ([d6d299d](https://github.com/0xPlayerOne/code-foundry/commit/d6d299dd5b073d6a5e13ffc2aa016d856208d2e4))

## [1.51.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.50.1...v1.51.0) (2026-10-29)


### Features

* **release:** preserve caller publication overrides ([#795](https://github.com/0xPlayerOne/code-foundry/issues/795)) ([e49d2ba](https://github.com/0xPlayerOne/code-foundry/commit/e49d2bac4f8995808bfc6a726b0c2ff1e93c2a5f))

## [1.50.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.50.0...v1.50.1) (2026-10-29)


### Bug Fixes

* **sync:** replace complete consumer runtime ref ([#793](https://github.com/0xPlayerOne/code-foundry/issues/793)) ([6a0b5ef](https://github.com/0xPlayerOne/code-foundry/commit/6a0b5ef4f9a02c781745fa64f2f9748ea679f2d5))

## [1.50.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.49.3...v1.50.0) (2026-10-29)


### Features

* **release:** support npm OIDC publishing ([#791](https://github.com/0xPlayerOne/code-foundry/issues/791)) ([74b5155](https://github.com/0xPlayerOne/code-foundry/commit/74b5155157b9f163d70b00b138673c981e19c925))

## [1.49.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.49.2...v1.49.3) (2026-10-29)


### CI

* **validation:** require release checks until evidence exists ([#789](https://github.com/0xPlayerOne/code-foundry/issues/789)) ([a5f8be6](https://github.com/0xPlayerOne/code-foundry/commit/a5f8be64b7b28d2248aa71b80e321aa0fe82f30a))

## [1.49.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.49.1...v1.49.2) (2026-10-29)


### Bug Fixes

* safely categorize npm publication failures ([#787](https://github.com/0xPlayerOne/code-foundry/issues/787)) ([a4268af](https://github.com/0xPlayerOne/code-foundry/commit/a4268af5ce7cd0a32407420424419c0cad01dce8))

## [1.49.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.49.0...v1.49.1) (2026-10-28)


### Bug Fixes

* handle empty security audit matrices ([#785](https://github.com/0xPlayerOne/code-foundry/issues/785)) ([02f0565](https://github.com/0xPlayerOne/code-foundry/commit/02f05652e68267a2aa2df5d5af8f13df9ba1e3aa))

## [1.49.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.9...v1.49.0) (2026-10-27)


### Features

* support isolated integration test shards ([#783](https://github.com/0xPlayerOne/code-foundry/issues/783)) ([ad1123f](https://github.com/0xPlayerOne/code-foundry/commit/ad1123ff3bb9654bfbdaef4219490cca3e7e3d20))

## [1.48.9](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.8...v1.48.9) (2026-10-26)


### Bug Fixes

* **release:** preserve fallback stdin and paginate existing releases ([#781](https://github.com/0xPlayerOne/code-foundry/issues/781)) ([ede4d2c](https://github.com/0xPlayerOne/code-foundry/commit/ede4d2c7e3bc7d1174580c9a0bc83bdaa160c2da))

## [1.48.8](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.7...v1.48.8) (2026-10-24)


### Bug Fixes

* **release:** hydrate audit blobs and refresh changing PR state ([#779](https://github.com/0xPlayerOne/code-foundry/issues/779)) ([8734ed7](https://github.com/0xPlayerOne/code-foundry/commit/8734ed77d159818cd5ff613f40a5dab796789d8a))

## [1.48.7](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.6...v1.48.7) (2026-10-23)


### Bug Fixes

* **release:** sync bun.lock workspace versions on generated release PRs ([#777](https://github.com/0xPlayerOne/code-foundry/issues/777)) ([b24bfae](https://github.com/0xPlayerOne/code-foundry/commit/b24bfae309ac7003fcc4cd57f79ddc418c27b039))

## [1.48.6](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.5...v1.48.6) (2026-10-23)


### Bug Fixes

* **release:** audit generated release content for stale snapshots ([#775](https://github.com/0xPlayerOne/code-foundry/issues/775)) ([f842c27](https://github.com/0xPlayerOne/code-foundry/commit/f842c271e6b270b63a6d9b839795a849237c7a7d))

## [1.48.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.4...v1.48.5) (2026-10-22)


### Bug Fixes

* **ci:** serialize billing receipt and report uploads ([#773](https://github.com/0xPlayerOne/code-foundry/issues/773)) ([6497225](https://github.com/0xPlayerOne/code-foundry/commit/6497225bf2d672380b6b5231378b424dffb8afbb))

## [1.48.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.3...v1.48.4) (2026-10-22)


### Maintenance

* bun-1.4.4-cloud ([#771](https://github.com/0xPlayerOne/code-foundry/issues/771)) ([c99f0ed](https://github.com/0xPlayerOne/code-foundry/commit/c99f0ed8b66129f3b599326bc67d900719b921f4))

## [1.48.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.2...v1.48.3) (2026-10-17)


### Tests

* read the chained hook fixture with fs.readFileSync ([#769](https://github.com/0xPlayerOne/code-foundry/issues/769)) ([5d5925a](https://github.com/0xPlayerOne/code-foundry/commit/5d5925ac38975f5b1cc9b0785aa492db029e420c))

## [1.48.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.1...v1.48.2) (2026-10-17)


### Maintenance

* **bun:** align Bun runtime pins to 1.4.3 ([#767](https://github.com/0xPlayerOne/code-foundry/issues/767)) ([402343f](https://github.com/0xPlayerOne/code-foundry/commit/402343fed2b41be3b2a55ddbc56d2256cc511b1a))

## [1.48.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.48.0...v1.48.1) (2026-10-16)


### Bug Fixes

* vite-plus-cache-post-job-save ([#765](https://github.com/0xPlayerOne/code-foundry/issues/765)) ([3f82e85](https://github.com/0xPlayerOne/code-foundry/commit/3f82e850f5c09af6cea4de6f1a791d098bbd2f6e))

## [1.48.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.47.5...v1.48.0) (2026-10-16)


### Features

* add opt-in Vite+ task runner support ([#763](https://github.com/0xPlayerOne/code-foundry/issues/763)) ([f7970cd](https://github.com/0xPlayerOne/code-foundry/commit/f7970cdf1c1880aaee159d2de79ba043f93711a7))

## [1.47.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.47.4...v1.47.5) (2026-10-15)


### Bug Fixes

* validation-issue-read-v1471 ([#759](https://github.com/0xPlayerOne/code-foundry/issues/759)) ([7119b3e](https://github.com/0xPlayerOne/code-foundry/commit/7119b3e2baebfbfdd47d32428cbf5df2f2079afa))

## [1.47.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.47.3...v1.47.4) (2026-10-15)


### Documentation

* fix generated agent contribution and validation references ([#760](https://github.com/0xPlayerOne/code-foundry/issues/760)) ([c3564c9](https://github.com/0xPlayerOne/code-foundry/commit/c3564c92cb168449317afe2e40359144bf7a0c71))

## [1.47.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.47.2...v1.47.3) (2026-10-09)


### Maintenance

* **fleet:** point the manifest at the rollout worktrees and filter adea's actionlint ([#757](https://github.com/0xPlayerOne/code-foundry/issues/757)) ([55bae8b](https://github.com/0xPlayerOne/code-foundry/commit/55bae8bf99a022bfa03294972d89a3cca20a6203))

## [1.47.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.47.1...v1.47.2) (2026-10-08)


### Bug Fixes

* **qualification:** exclude pending parallel syntax by content, not filename ([#755](https://github.com/0xPlayerOne/code-foundry/issues/755)) ([1f7cae8](https://github.com/0xPlayerOne/code-foundry/commit/1f7cae8167002061850e56e3dc0fa800a69d7be9))

## [1.47.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.47.0...v1.47.1) (2026-10-08)


### Tests

* **doctor:** pin the machine-hook shadow warning ([#753](https://github.com/0xPlayerOne/code-foundry/issues/753)) ([f634269](https://github.com/0xPlayerOne/code-foundry/commit/f634269424580d8d34323319288747587b6d6ae3))

## [1.47.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.46.6...v1.47.0) (2026-10-08)


### Features

* **release:** configurable dev channel on top of batched releases ([#749](https://github.com/0xPlayerOne/code-foundry/issues/749)) ([8fd8556](https://github.com/0xPlayerOne/code-foundry/commit/8fd85567a1a89735ab0db589649741253fbbeb21)), closes [#699](https://github.com/0xPlayerOne/code-foundry/issues/699)

## [1.46.6](https://github.com/0xPlayerOne/code-foundry/compare/v1.46.5...v1.46.6) (2026-10-08)


### Bug Fixes

* **pre-commit:** build before lint and type-check when the gate opts in ([#748](https://github.com/0xPlayerOne/code-foundry/issues/748)) ([f56454f](https://github.com/0xPlayerOne/code-foundry/commit/f56454f313a1a5b802b8a17b09d850902de1ba55)), closes [#691](https://github.com/0xPlayerOne/code-foundry/issues/691)

## [1.46.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.46.4...v1.46.5) (2026-10-08)


### Bug Fixes

* **sync:** chain machine-level hooks instead of silencing them ([#747](https://github.com/0xPlayerOne/code-foundry/issues/747)) ([7fcad52](https://github.com/0xPlayerOne/code-foundry/commit/7fcad52d400dbb2aaa9ba46c0c76f14e8d63f660)), closes [#690](https://github.com/0xPlayerOne/code-foundry/issues/690)

## [1.46.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.46.3...v1.46.4) (2026-10-08)


### Bug Fixes

* **release:** preserve current-head validation ownership ([#737](https://github.com/0xPlayerOne/code-foundry/issues/737)) ([aa8bfcf](https://github.com/0xPlayerOne/code-foundry/commit/aa8bfcfbfcd3c213d15ba9e1fbfb5c65ab8ddb6b))

## [1.46.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.46.2...v1.46.3) (2026-10-07)


### Bug Fixes

* **billing:** keep lint standalone; join fast-lane receipts in parallel ([#744](https://github.com/0xPlayerOne/code-foundry/issues/744)) ([574690b](https://github.com/0xPlayerOne/code-foundry/commit/574690b707abffe9350ccc67589540afb82323ee))

## [1.46.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.46.1...v1.46.2) (2026-10-07)


### Bug Fixes

* **billing:** join fast-lane receipts in a second parallel group ([#742](https://github.com/0xPlayerOne/code-foundry/issues/742)) ([c63a39c](https://github.com/0xPlayerOne/code-foundry/commit/c63a39cf5e236d6747bd85cf10b04bd10f690b11))

## [1.46.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.46.0...v1.46.1) (2026-10-07)


### Bug Fixes

* **qualification:** skip parallel-syntax files until actionlint supports them ([#740](https://github.com/0xPlayerOne/code-foundry/issues/740)) ([db98c7f](https://github.com/0xPlayerOne/code-foundry/commit/db98c7f40cae080cdc9dcab7baac4976e5e0656e))

## [1.46.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.45.2...v1.46.0) (2026-10-07)


### Features

* **billing:** run fast-lane executes concurrently ([#738](https://github.com/0xPlayerOne/code-foundry/issues/738)) ([b40e82a](https://github.com/0xPlayerOne/code-foundry/commit/b40e82a0709b288a8be46998cfdc8b909f92c23c))

## [1.45.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.45.1...v1.45.2) (2026-10-06)


### Bug Fixes

* **billing:** emit the codeql input as a YAML boolean ([#735](https://github.com/0xPlayerOne/code-foundry/issues/735)) ([e0b348c](https://github.com/0xPlayerOne/code-foundry/commit/e0b348c9a3c730e46210fe0b9dc46af49c9db605))

## [1.45.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.45.0...v1.45.1) (2026-10-06)


### Bug Fixes

* **billing:** declare the runner inputs the callers always forward ([#733](https://github.com/0xPlayerOne/code-foundry/issues/733)) ([f7a29cb](https://github.com/0xPlayerOne/code-foundry/commit/f7a29cb6dbc9a8695a9bef9e85ccce82aa9c84db))

## [1.45.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.11...v1.45.0) (2026-10-06)


### Features

* add a merged-lane billing orchestrator for minute-billed consumers ([#731](https://github.com/0xPlayerOne/code-foundry/issues/731)) ([a91402e](https://github.com/0xPlayerOne/code-foundry/commit/a91402e701f458ece0d2ea4715f9586a06b15108))

## [1.44.11](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.10...v1.44.11) (2026-10-06)


### Bug Fixes

* **release:** retry the token probe and REST fallback writes with backoff ([#729](https://github.com/0xPlayerOne/code-foundry/issues/729)) ([ad28e18](https://github.com/0xPlayerOne/code-foundry/commit/ad28e18326f0ee8c25950fb649eb81cdb3dc0a1a))

## [1.44.10](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.9...v1.44.10) (2026-10-06)


### Bug Fixes

* **release:** treat ref-creation errors in the REST fallback as non-fatal ([#727](https://github.com/0xPlayerOne/code-foundry/issues/727)) ([75ea614](https://github.com/0xPlayerOne/code-foundry/commit/75ea61465e7c4cacd39e3aa8c52df93c2ea9bf03))

## [1.44.9](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.8...v1.44.9) (2026-10-06)


### Bug Fixes

* **release:** make the REST fallback draft-aware and idempotent ([#725](https://github.com/0xPlayerOne/code-foundry/issues/725)) ([c29da6e](https://github.com/0xPlayerOne/code-foundry/commit/c29da6efb919d68a568c2328eea2c2f7654334fe))

## [1.44.8](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.7...v1.44.8) (2026-10-06)


### Bug Fixes

* **release:** query the version-PR branch directly in the REST fallback ([#722](https://github.com/0xPlayerOne/code-foundry/issues/722)) ([b38f394](https://github.com/0xPlayerOne/code-foundry/commit/b38f394c0ca6438117fdd2f45bd106b0b145a0f9))

## [1.44.7](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.6...v1.44.7) (2026-10-05)


### Bug Fixes

* **release:** complete rejected release-please runs over REST ([#720](https://github.com/0xPlayerOne/code-foundry/issues/720)) ([14e88b5](https://github.com/0xPlayerOne/code-foundry/commit/14e88b5561803fc8d5d3a77b67b99e1be90bc4af))

## [1.44.6](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.5...v1.44.6) (2026-10-05)


### Bug Fixes

* **config:** pin the lint-bearing CI lane to a standard runner by default ([#718](https://github.com/0xPlayerOne/code-foundry/issues/718)) ([fc0ed14](https://github.com/0xPlayerOne/code-foundry/commit/fc0ed14434151fb11eef7c0d4c324c7a370d5058))

## [1.44.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.4...v1.44.5) (2026-10-05)


### Bug Fixes

* **release:** probe the tag-creation write before trusting the automation token ([#716](https://github.com/0xPlayerOne/code-foundry/issues/716)) ([fabaddc](https://github.com/0xPlayerOne/code-foundry/commit/fabaddcb05d5dc701248b693f91be6ee433f8d39))

## [1.44.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.3...v1.44.4) (2026-10-03)


### Bug Fixes

* **ci:** declare the e2e shard inputs on the no-codeql orchestrator ([#714](https://github.com/0xPlayerOne/code-foundry/issues/714)) ([7500208](https://github.com/0xPlayerOne/code-foundry/commit/7500208f3b25dfe55c41ea45b382e021cf804012))

## [1.44.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.2...v1.44.3) (2026-10-03)


### Tests

* **cli:** assert expected doctor warnings ([#712](https://github.com/0xPlayerOne/code-foundry/issues/712)) ([d036bee](https://github.com/0xPlayerOne/code-foundry/commit/d036beee79a9b200315cdbee5509fc3c2a6c4a04))

## [1.44.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.1...v1.44.2) (2026-10-03)


### Bug Fixes

* **ci:** cancel only superseded pull-request runs in managed workflows ([#710](https://github.com/0xPlayerOne/code-foundry/issues/710)) ([f5fead6](https://github.com/0xPlayerOne/code-foundry/commit/f5fead677c032d253f2e1a2a256da4f207ddfa2a))

## [1.44.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.44.0...v1.44.1) (2026-10-03)


### Bug Fixes

* **release:** budget the package without the changelog and ship recent history only ([#708](https://github.com/0xPlayerOne/code-foundry/issues/708)) ([ab365e0](https://github.com/0xPlayerOne/code-foundry/commit/ab365e0910472c3596429adc86a1c8f3e19730f9))

## [1.44.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.43.2...v1.44.0) (2026-10-03)


### Features

* **pre-commit:** make the commit gate change-aware ([#702](https://github.com/0xPlayerOne/code-foundry/issues/702)) ([f5bca91](https://github.com/0xPlayerOne/code-foundry/commit/f5bca91c177b30b99f5d62287255d191617b4788))

## [1.43.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.43.1...v1.43.2) (2026-10-03)


### Bug Fixes

* require candidate asset qualification before stable promotion ([#705](https://github.com/0xPlayerOne/code-foundry/issues/705)) ([f42e4f5](https://github.com/0xPlayerOne/code-foundry/commit/f42e4f5fb063ea22fa25791a13c75c90d41bf17a))

## [1.43.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.43.0...v1.43.1) (2026-10-03)


### Bug Fixes

* **release:** make batched publication and stable promotion reliable ([#703](https://github.com/0xPlayerOne/code-foundry/issues/703)) ([271731d](https://github.com/0xPlayerOne/code-foundry/commit/271731d8fac3bff42a99b3d5f4a774eccc0a7788))

## [1.43.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.42.0...v1.43.0) (2026-10-03)


### Features

* release-batching ([#700](https://github.com/0xPlayerOne/code-foundry/issues/700)) ([3dd5c5f](https://github.com/0xPlayerOne/code-foundry/commit/3dd5c5fd50883608baa3e2f9daef6b8aa83f269f))

## [1.42.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.41.0...v1.42.0) (2026-10-02)


### Features

* **validation:** shard the managed E2E lane via e2e_shards ([#697](https://github.com/0xPlayerOne/code-foundry/issues/697)) ([edb20b4](https://github.com/0xPlayerOne/code-foundry/commit/edb20b4e32e2055bf22e6f6f94b51f234a24687d))

## [1.41.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.40.0...v1.41.0) (2026-10-02)


### Features

* **validation:** skip default-branch CodeQL on release-please merges ([#694](https://github.com/0xPlayerOne/code-foundry/issues/694)) ([25fc22e](https://github.com/0xPlayerOne/code-foundry/commit/25fc22e6d4b76f0b7e06601f6dc420085949f127))


### Bug Fixes

* give the release artifact budgets several releases of headroom ([#696](https://github.com/0xPlayerOne/code-foundry/issues/696)) ([a504607](https://github.com/0xPlayerOne/code-foundry/commit/a504607e16f097a5075191fd24cb26953b06a340))

## [1.40.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.39.3...v1.40.0) (2026-10-02)


### Features

* **sync:** add dependency_updater setting to gate Dependabot and scaffold Renovate ([#692](https://github.com/0xPlayerOne/code-foundry/issues/692)) ([15805de](https://github.com/0xPlayerOne/code-foundry/commit/15805dee09a93ca168bbc00dbc3c3af36a40e7bf))

## [1.39.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.39.2...v1.39.3) (2026-10-01)


### Bug Fixes

* **hooks:** run the gate from a local dependency, not npx ([#688](https://github.com/0xPlayerOne/code-foundry/issues/688)) ([d256b69](https://github.com/0xPlayerOne/code-foundry/commit/d256b69b8f89f0041a01c53cc51af32fe582b5dc))

## [1.39.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.39.1...v1.39.2) (2026-10-01)


### Bug Fixes

* **hooks:** delegate the generated pre-commit hook to the runtime ([#684](https://github.com/0xPlayerOne/code-foundry/issues/684)) ([5d9a571](https://github.com/0xPlayerOne/code-foundry/commit/5d9a5714aeff0d48397e3be51b22e08395bfb5ce))

## [1.39.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.39.0...v1.39.1) (2026-10-01)


### Bug Fixes

* report inactive main rulesets in github doctor ([#682](https://github.com/0xPlayerOne/code-foundry/issues/682)) ([695a0b4](https://github.com/0xPlayerOne/code-foundry/commit/695a0b437910aa8e664a481c1648dbadcc1a2de8))

## [1.39.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.38.1...v1.39.0) (2026-10-01)


### Features

* **ci:** surface ungated scheduled workflows in the billing pause controls ([#681](https://github.com/0xPlayerOne/code-foundry/issues/681)) ([ef48f9a](https://github.com/0xPlayerOne/code-foundry/commit/ef48f9a25aa0b22f82b0ed8a512bc1a65d08d8e9))


### Maintenance

* register the adea-ai ui and themes consumers in the fleet manifest ([#680](https://github.com/0xPlayerOne/code-foundry/issues/680)) ([f50e6c6](https://github.com/0xPlayerOne/code-foundry/commit/f50e6c6a4ef4b7f0396cdce21f53070fec818c50))

## [1.38.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.38.0...v1.38.1) (2026-09-30)


### Bug Fixes

* normalize blank runs when stripping legacy managed markers ([#678](https://github.com/0xPlayerOne/code-foundry/issues/678)) ([acd5afc](https://github.com/0xPlayerOne/code-foundry/commit/acd5afce12b3de3b3574259639e89067e1ab3cb0))

## [1.38.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.37.3...v1.38.0) (2026-09-30)


### Features

* fold the Turbo impact check into the delivery candidate job ([#676](https://github.com/0xPlayerOne/code-foundry/issues/676)) ([fd99d29](https://github.com/0xPlayerOne/code-foundry/commit/fd99d29ae7e10ef9346b8059dcad0ed4df6df109))

## [1.37.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.37.2...v1.37.3) (2026-09-30)


### Bug Fixes

* perf-budget-best-of-n ([#674](https://github.com/0xPlayerOne/code-foundry/issues/674)) ([c377ede](https://github.com/0xPlayerOne/code-foundry/commit/c377ede617d89fb0606413ab7b5d478330c49e93))

## [1.37.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.37.1...v1.37.2) (2026-09-30)


### Bug Fixes

* **cloudflare:** surface the cf deploy error instead of discarding it ([66de0d1](https://github.com/0xPlayerOne/code-foundry/commit/66de0d1e8238315dbd910abbd907e921cbc6764f))

## [1.37.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.37.0...v1.37.1) (2026-09-30)


### Bug Fixes

* **cloudflare:** build the production Build Output before the prebuilt deploy ([5f2f83c](https://github.com/0xPlayerOne/code-foundry/commit/5f2f83c6d6135c403b520f83469c0c5ca350cdba))

## [1.37.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.36.4...v1.37.0) (2026-09-30)


### Features

* preserve repository-owned sections of managed policy documents ([#668](https://github.com/0xPlayerOne/code-foundry/issues/668)) ([26e9f4b](https://github.com/0xPlayerOne/code-foundry/commit/26e9f4bfeaca8b01087626bafbfc5090d891530f)), closes [#667](https://github.com/0xPlayerOne/code-foundry/issues/667)

## [1.36.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.36.3...v1.36.4) (2026-09-29)


### Bug Fixes

* **cloudflare:** deploy previews from the prebuilt Preview Build Output ([#664](https://github.com/0xPlayerOne/code-foundry/issues/664)) ([34966ea](https://github.com/0xPlayerOne/code-foundry/commit/34966ea3917c145c441a460c741c125c60f84d25))

## [1.36.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.36.2...v1.36.3) (2026-09-29)


### Maintenance

* track the JavaScript Dependabot ecosystem as bun by default ([#648](https://github.com/0xPlayerOne/code-foundry/issues/648)) ([6aa9712](https://github.com/0xPlayerOne/code-foundry/commit/6aa9712904340a7e4783f697a0e02d2be6ab1dce))

## [1.36.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.36.1...v1.36.2) (2026-09-29)


### Bug Fixes

* **cloudflare:** resolve cf bins by walking up node_modules/.bin ([#662](https://github.com/0xPlayerOne/code-foundry/issues/662)) ([e82bbe0](https://github.com/0xPlayerOne/code-foundry/commit/e82bbe0a1687b5cc8bf939769e15639f25199969))

## [1.36.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.36.0...v1.36.1) (2026-09-29)


### Bug Fixes

* **cloudflare:** build a preview Build Output before cf previews deploy ([#660](https://github.com/0xPlayerOne/code-foundry/issues/660)) ([d897380](https://github.com/0xPlayerOne/code-foundry/commit/d897380110a692143b3bcb0915d8ce40cff4663c))

## [1.36.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.35.0...v1.36.0) (2026-09-29)


### Features

* **cloudflare:** add a cf deploy mode to cloudflare-deploy.yml ([#658](https://github.com/0xPlayerOne/code-foundry/issues/658)) ([31ef8ca](https://github.com/0xPlayerOne/code-foundry/commit/31ef8ca607c189d7ca0bbe4f42de85ee27edabc9))

## [1.35.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.34.0...v1.35.0) (2026-09-29)


### Features

* fold the Turbo impact check into the cloudflare deploy job ([#655](https://github.com/0xPlayerOne/code-foundry/issues/655)) ([b72f5f2](https://github.com/0xPlayerOne/code-foundry/commit/b72f5f26f045103755bb2795f2fc3a84e7625b3c))
* scope CodeQL analysis to changed languages and Rust shards on pull requests ([#654](https://github.com/0xPlayerOne/code-foundry/issues/654)) ([d5ce743](https://github.com/0xPlayerOne/code-foundry/commit/d5ce74377601c2efb3be4831320cb62cdfbd999b))
* skip the security detector entirely while OpenCode Security is disabled ([#653](https://github.com/0xPlayerOne/code-foundry/issues/653)) ([9e4271e](https://github.com/0xPlayerOne/code-foundry/commit/9e4271e597d65b4f63c571baab5507eacaab1ce5))


### Maintenance

* raise the packed artifact budget to 286 kB ([#657](https://github.com/0xPlayerOne/code-foundry/issues/657)) ([4512af7](https://github.com/0xPlayerOne/code-foundry/commit/4512af75fc18a36292f495c5e7f51791ba38f3d6))

## [1.34.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.33.3...v1.34.0) (2026-09-29)


### Features

* billing-paused-dependabot ([#651](https://github.com/0xPlayerOne/code-foundry/issues/651)) ([eda05b5](https://github.com/0xPlayerOne/code-foundry/commit/eda05b5cfa28fc7314ec33a94e539a1660549511))

## [1.33.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.33.2...v1.33.3) (2026-09-29)


### Bug Fixes

* **ci:** launch wrangler under Node in the cloudflare deploy step ([#649](https://github.com/0xPlayerOne/code-foundry/issues/649)) ([e797934](https://github.com/0xPlayerOne/code-foundry/commit/e7979343d3ff4d1fe5dc1520568a501cce0c47f3))

## [1.33.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.33.1...v1.33.2) (2026-09-26)


### Bug Fixes

* **release:** queue version PR merges on branch policy ([#646](https://github.com/0xPlayerOne/code-foundry/issues/646)) ([ca492c8](https://github.com/0xPlayerOne/code-foundry/commit/ca492c8402bfc43ef718c0a6443ee06fcb33e957))

## [1.33.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.33.0...v1.33.1) (2026-09-25)


### Bug Fixes

* **security:** stop a clean pip-audit result from failing the audit gate ([#643](https://github.com/0xPlayerOne/code-foundry/issues/643)) ([7260291](https://github.com/0xPlayerOne/code-foundry/commit/7260291fc24e851678ddbf9cc9dfcf99bea48f59))


### Maintenance

* **perf:** recalibrate the packed artifact budget ([#645](https://github.com/0xPlayerOne/code-foundry/issues/645)) ([64b6504](https://github.com/0xPlayerOne/code-foundry/commit/64b65049ba313f01f6989bf52a83efe31d2b91dd))

## [1.33.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.32.0...v1.33.0) (2026-09-22)


### Features

* **cloudflare-deploy:** accept optional TURBO_TOKEN secret for remote-cached deploy builds ([#640](https://github.com/0xPlayerOne/code-foundry/issues/640)) ([091bfd1](https://github.com/0xPlayerOne/code-foundry/commit/091bfd12b6bbca0e9289a74827713dc50bcb4193))

## [1.32.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.31.0...v1.32.0) (2026-09-21)


### Features

* forward TURBO_API to validation and cloudflare deploy builds ([#638](https://github.com/0xPlayerOne/code-foundry/issues/638)) ([55347f6](https://github.com/0xPlayerOne/code-foundry/commit/55347f6fd3bea41f11aa936650222cd73cfd8026))

## [1.31.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.30.2...v1.31.0) (2026-09-21)


### Features

* **cloudflare-deploy:** cache the Bun package cache across deploy jobs ([#636](https://github.com/0xPlayerOne/code-foundry/issues/636)) ([42048b8](https://github.com/0xPlayerOne/code-foundry/commit/42048b8ec7130c89d35cd93568d720098c37d773))

## [1.30.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.30.1...v1.30.2) (2026-09-17)


### Maintenance

* adopt Code Foundry runtime v1.30.0 ([#634](https://github.com/0xPlayerOne/code-foundry/issues/634)) ([2d6d6c9](https://github.com/0xPlayerOne/code-foundry/commit/2d6d6c96a98603dc1394356d01802ca551482ae4))

## [1.30.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.30.0...v1.30.1) (2026-09-17)


### Maintenance

* toolchain-alignment ([#630](https://github.com/0xPlayerOne/code-foundry/issues/630)) ([0d0ddbe](https://github.com/0xPlayerOne/code-foundry/commit/0d0ddbe9f6cbee65094360ff1cd4aadab845b326))

## [1.30.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.29.1...v1.30.0) (2026-09-17)


### Features

* resolve lane diffs only for filtered lanes and accept injected paths ([#631](https://github.com/0xPlayerOne/code-foundry/issues/631)) ([04a0d8a](https://github.com/0xPlayerOne/code-foundry/commit/04a0d8a69b3fd3d3417eef46e22e0eb79860fb04))

## [1.29.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.29.0...v1.29.1) (2026-09-17)


### Maintenance

* align oxlint and oxfmt pins with fleet standard ([#628](https://github.com/0xPlayerOne/code-foundry/issues/628)) ([32c88f1](https://github.com/0xPlayerOne/code-foundry/commit/32c88f153e06e1f1eda61b16fcb0ba50a847a99a))

## [1.29.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.15...v1.29.0) (2026-09-17)


### Features

* opt-in lane path filters, sccache, and nextest for Rust CI ([#626](https://github.com/0xPlayerOne/code-foundry/issues/626)) ([691ccad](https://github.com/0xPlayerOne/code-foundry/commit/691ccad529d88cde4ddd134b30cfb86988a1cb0a))

## [1.28.15](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.14...v1.28.15) (2026-09-17)


### Bug Fixes

* **codeql:** analyze the pull request head commit ([#624](https://github.com/0xPlayerOne/code-foundry/issues/624)) ([ce05d1f](https://github.com/0xPlayerOne/code-foundry/commit/ce05d1f4f6c5df3a2d9134dd4657f478a265cb85))

## [1.28.14](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.13...v1.28.14) (2026-09-11)


### Bug Fixes

* **sync:** accept mixed broad and scoped CodeQL Rust shards ([#621](https://github.com/0xPlayerOne/code-foundry/issues/621)) ([f13c5a7](https://github.com/0xPlayerOne/code-foundry/commit/f13c5a734a1b24ee75566bab3b778052a28ada99))

## [1.28.13](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.12...v1.28.13) (2026-09-11)


### Bug Fixes

* **fleet:** accept base-config evidence for merged rollouts ([#620](https://github.com/0xPlayerOne/code-foundry/issues/620)) ([394c528](https://github.com/0xPlayerOne/code-foundry/commit/394c528a137617ce2c4464436dbc6068349a0c54))

## [1.28.12](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.11...v1.28.12) (2026-09-11)


### Maintenance

* **fleet:** add explicit inventory manifest ([#618](https://github.com/0xPlayerOne/code-foundry/issues/618)) ([0771878](https://github.com/0xPlayerOne/code-foundry/commit/077187817728f3d4eb40333b6e6d07fa533a9780))

## [1.28.11](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.10...v1.28.11) (2026-09-11)


### Bug Fixes

* **fleet:** bound rendered jobs with timeouts and refresh stale runtime pins ([#616](https://github.com/0xPlayerOne/code-foundry/issues/616)) ([f8d20b4](https://github.com/0xPlayerOne/code-foundry/commit/f8d20b4ad48cddd20630ff9b7c1c21d0c5ac9520))

## [1.28.10](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.9...v1.28.10) (2026-09-11)


### Bug Fixes

* **ci:** dedupe caller names and keep CodeQL Rust shards aligned ([#613](https://github.com/0xPlayerOne/code-foundry/issues/613)) ([8000e5e](https://github.com/0xPlayerOne/code-foundry/commit/8000e5e152ccc7e657933b55eb5b82a278762176))

## [1.28.9](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.8...v1.28.9) (2026-09-11)


### Bug Fixes

* **sync:** render the configured Rust shards into every CodeQL lane ([#612](https://github.com/0xPlayerOne/code-foundry/issues/612)) ([4e7eb2f](https://github.com/0xPlayerOne/code-foundry/commit/4e7eb2f03ba34b4fe459e8ce302bcbf3303b26cc))

## [1.28.8](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.7...v1.28.8) (2026-09-11)


### Bug Fixes

* **deploy:** send auto_inactive once when completing a deployment status ([#610](https://github.com/0xPlayerOne/code-foundry/issues/610)) ([9951887](https://github.com/0xPlayerOne/code-foundry/commit/99518875f584e08cbd2b52759f13fc6065bcd1c5))

## [1.28.7](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.6...v1.28.7) (2026-09-11)


### Bug Fixes

* **delivery:** drop impossible NUL guard that always failed the turbo impact check ([#607](https://github.com/0xPlayerOne/code-foundry/issues/607)) ([211db01](https://github.com/0xPlayerOne/code-foundry/commit/211db01cda6fc4f3f6f660b0a807c4cd921cc877))

## [1.28.6](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.5...v1.28.6) (2026-09-10)


### Bug Fixes

* **sync:** preserve non-CodeQL workflow triggers ([#605](https://github.com/0xPlayerOne/code-foundry/issues/605)) ([e215207](https://github.com/0xPlayerOne/code-foundry/commit/e215207d596361f283072d4f43f8ab58676e13c8))

## [1.28.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.4...v1.28.5) (2026-09-10)


### Bug Fixes

* **fleet:** require explicit inventory manifest ([#603](https://github.com/0xPlayerOne/code-foundry/issues/603)) ([1345331](https://github.com/0xPlayerOne/code-foundry/commit/13453318ba4fb21e6df6d978f1d51119148300ba))

## [1.28.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.3...v1.28.4) (2026-09-10)


### Bug Fixes

* **release:** scope reconciliation to staging topology ([bfba0c1](https://github.com/0xPlayerOne/code-foundry/commit/bfba0c147ea6281c47754938d6711d3e5e0335a2))

## [1.28.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.2...v1.28.3) (2026-09-10)


### Maintenance

* **config:** pin Code Foundry runtime to v1.28.2 ([#599](https://github.com/0xPlayerOne/code-foundry/issues/599)) ([ed61358](https://github.com/0xPlayerOne/code-foundry/commit/ed6135813e12e1f5410066a92183f2f2d18dcc8c))

## [1.28.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.1...v1.28.2) (2026-09-10)


### Bug Fixes

* **release:** pass one qualification report per required node ([#597](https://github.com/0xPlayerOne/code-foundry/issues/597)) ([5ceb92c](https://github.com/0xPlayerOne/code-foundry/commit/5ceb92cab3afc97145ef068e6b5e33399d99b9e5))

## [1.28.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.28.0...v1.28.1) (2026-09-10)


### Bug Fixes

* **cloudflare:** remove duplicate deployment records ([#595](https://github.com/0xPlayerOne/code-foundry/issues/595)) ([d9a2a4b](https://github.com/0xPlayerOne/code-foundry/commit/d9a2a4b0363bb9a9ded91d3368bdb7b9b580330f))

## [1.28.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.27.0...v1.28.0) (2026-09-10)


### Features

* **release:** qualify only when a release or a stuck draft needs it ([#591](https://github.com/0xPlayerOne/code-foundry/issues/591)) ([4cce045](https://github.com/0xPlayerOne/code-foundry/commit/4cce045228648e6e705ad1e89c59eaf20a72a538))

## [1.27.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.26.0...v1.27.0) (2026-09-10)


### Features

* **validation:** downgrade docs-only PRs to fast and gate bot pushes ([#590](https://github.com/0xPlayerOne/code-foundry/issues/590)) ([df774f5](https://github.com/0xPlayerOne/code-foundry/commit/df774f5d1e4a8a6c5f174219eb2b24ef012f6fd3))

## [1.26.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.25.3...v1.26.0) (2026-09-10)


### Features

* **node:** support Node 24 and 26, drop 20 and 22 ([#589](https://github.com/0xPlayerOne/code-foundry/issues/589)) ([ee3e294](https://github.com/0xPlayerOne/code-foundry/commit/ee3e2943889ffd06a8d4cd4ccb75a3f36c46c0fd))

## [1.25.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.25.2...v1.25.3) (2026-09-10)


### Bug Fixes

* **release:** cover the attestation lag in publication retries ([#587](https://github.com/0xPlayerOne/code-foundry/issues/587)) ([7ae5e4b](https://github.com/0xPlayerOne/code-foundry/commit/7ae5e4bb95f68cbf4e2b48778776a0396c877271))

## [1.25.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.25.1...v1.25.2) (2026-09-10)


### Bug Fixes

* **release:** retry integrity verification through the publication consistency window ([#585](https://github.com/0xPlayerOne/code-foundry/issues/585)) ([5b997dd](https://github.com/0xPlayerOne/code-foundry/commit/5b997dda7e272b59a386eeeda115e60ad284f6ce))

## [1.25.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.25.0...v1.25.1) (2026-09-10)


### Bug Fixes

* **release:** wait for the release index before verifying a published release ([#583](https://github.com/0xPlayerOne/code-foundry/issues/583)) ([7823c14](https://github.com/0xPlayerOne/code-foundry/commit/7823c1473d8c5e7c17b039dc755ff5c8d1dba39c))

## [1.25.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.24.0...v1.25.0) (2026-09-10)


### Features

* **eval:** run the eval tier as a managed Validation / Eval lane ([#580](https://github.com/0xPlayerOne/code-foundry/issues/580)) ([9414889](https://github.com/0xPlayerOne/code-foundry/commit/94148894da9a627a6bd7c71c846848c198c1dfec))

## [1.24.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.23.0...v1.24.0) (2026-09-10)


### Features

* **validation:** run a lean release lane for Release Please pull requests ([#579](https://github.com/0xPlayerOne/code-foundry/issues/579)) ([a38ca75](https://github.com/0xPlayerOne/code-foundry/commit/a38ca75c7da577af8368467b8b026d0ec563fc41))

## [1.23.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.22.1...v1.23.0) (2026-09-09)


### Features

* add ci eval tier with shared report contract and budget gate ([#576](https://github.com/0xPlayerOne/code-foundry/issues/576)) ([7d881dd](https://github.com/0xPlayerOne/code-foundry/commit/7d881dd1bc6ace8e48dffff45b1a22a12bdae1c9))

## [1.22.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.22.0...v1.22.1) (2026-09-09)


### Bug Fixes

* **release:** use shell-safe recovery script ([#574](https://github.com/0xPlayerOne/code-foundry/issues/574)) ([264036f](https://github.com/0xPlayerOne/code-foundry/commit/264036f34afa4d7bc405285918395f2ce075bde3))

## [1.22.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.21.3...v1.22.0) (2026-09-09)


### Features

* **workflows:** protect draft pull requests by default ([#572](https://github.com/0xPlayerOne/code-foundry/issues/572)) ([6fa4ce1](https://github.com/0xPlayerOne/code-foundry/commit/6fa4ce1b2dde5eddff361b819722912fed7a9815))

## [1.21.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.21.2...v1.21.3) (2026-09-09)


### Bug Fixes

* **release:** unblock draft publication and PR deployment links ([#570](https://github.com/0xPlayerOne/code-foundry/issues/570)) ([35ab90f](https://github.com/0xPlayerOne/code-foundry/commit/35ab90f185483b0cd6a9c622b9793e46c90dd60c))

## [1.21.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.21.1...v1.21.2) (2026-09-09)


### Documentation

* refresh documentation for current workflows ([#568](https://github.com/0xPlayerOne/code-foundry/issues/568)) ([d0028e0](https://github.com/0xPlayerOne/code-foundry/commit/d0028e096371e1019c466f72f8744bdf832e067c))

## [1.21.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.21.0...v1.21.1) (2026-09-09)


### Bug Fixes

* release-hook-and-performance-safety ([#565](https://github.com/0xPlayerOne/code-foundry/issues/565)) ([0d410c6](https://github.com/0xPlayerOne/code-foundry/commit/0d410c68abfbc0d9fdd03b7aa81676489e459c19))
* **release:** automate self publication after CI ([91b2655](https://github.com/0xPlayerOne/code-foundry/commit/91b265585aa03e742e5bfc8a839b2794bf234491))


### Performance

* **ci:** batch native Rust test targets by category ([#564](https://github.com/0xPlayerOne/code-foundry/issues/564)) ([6def882](https://github.com/0xPlayerOne/code-foundry/commit/6def8826e90b23d021a4f4587fa843dbb37df0e7))

## [1.21.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.20.2...v1.21.0) (2026-09-09)


### Features

* **release:** wire qualified draft staging and immutable publication ([#558](https://github.com/0xPlayerOne/code-foundry/issues/558)) ([19aea32](https://github.com/0xPlayerOne/code-foundry/commit/19aea32f50c747cdc5642d1752a9f02008c157f6))


### Bug Fixes

* **quality:** harden HTML filtering ([#562](https://github.com/0xPlayerOne/code-foundry/issues/562)) ([ea45590](https://github.com/0xPlayerOne/code-foundry/commit/ea45590db24dc05ef12db57e80c7405fa217514f))

## [1.20.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.20.1...v1.20.2) (2026-09-09)


### Bug Fixes

* **ci:** retain scoped task receipts across success and failure ([#557](https://github.com/0xPlayerOne/code-foundry/issues/557)) ([ee0fe45](https://github.com/0xPlayerOne/code-foundry/commit/ee0fe45e821621e3193831d70a533077b7bcf8a9))

## [1.20.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.20.0...v1.20.1) (2026-09-09)


### Bug Fixes

* **qualification:** isolate attempts and verify release handoff ([#556](https://github.com/0xPlayerOne/code-foundry/issues/556)) ([5fe7f42](https://github.com/0xPlayerOne/code-foundry/commit/5fe7f4203b8018fd3eb88bd68e2286c6feb3d3dc))

## [1.20.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.19.0...v1.20.0) (2026-09-09)


### Features

* **ci:** add opt-in merge-group audit validation ([#549](https://github.com/0xPlayerOne/code-foundry/issues/549)) ([ae418a7](https://github.com/0xPlayerOne/code-foundry/commit/ae418a779ada2927bd391cc6cf54db16e342d921))

## [1.19.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.18.0...v1.19.0) (2026-09-09)


### Features

* **fleet:** gate upgrades on verified release qualification ([#548](https://github.com/0xPlayerOne/code-foundry/issues/548)) ([3247cc6](https://github.com/0xPlayerOne/code-foundry/commit/3247cc6f2295c65c42bb43e4ec8f87a08f3dd02d))

## [1.18.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.17.0...v1.18.0) (2026-09-09)


### Features

* **releases:** stage qualified assets and publish verified identical archives ([#547](https://github.com/0xPlayerOne/code-foundry/issues/547)) ([dffcb83](https://github.com/0xPlayerOne/code-foundry/commit/dffcb834c8ee8c5c2bcba606350276e6a7de58d0))

## [1.17.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.16.0...v1.17.0) (2026-09-09)


### Features

* **quality:** add opt-in site, app, Worker, and package acceptance profiles ([#545](https://github.com/0xPlayerOne/code-foundry/issues/545)) ([1201793](https://github.com/0xPlayerOne/code-foundry/commit/1201793805b443c835b608609704bc43bcb035f5))

## [1.16.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.15.0...v1.16.0) (2026-09-09)


### Features

* **qualification:** gate releases on installed consumer compatibility ([#544](https://github.com/0xPlayerOne/code-foundry/issues/544)) ([33c759b](https://github.com/0xPlayerOne/code-foundry/commit/33c759be8c78c633f55a58dc6144986758676336))

## [1.15.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.14.0...v1.15.0) (2026-09-09)


### Features

* **releases:** verify immutable releases and attest selected build artifacts ([#537](https://github.com/0xPlayerOne/code-foundry/issues/537)) ([099aa57](https://github.com/0xPlayerOne/code-foundry/commit/099aa577227ab067a9a554e4cfc286aa2f5eb38e))

## [1.14.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.13.0...v1.14.0) (2026-09-09)


### Features

* **cli:** add shared validation plans and agent check evidence ([#538](https://github.com/0xPlayerOne/code-foundry/issues/538)) ([95af9ed](https://github.com/0xPlayerOne/code-foundry/commit/95af9ed42682ff3ed1dc74609ea4628d0c95a799))

## [1.13.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.12.0...v1.13.0) (2026-09-09)


### Features

* **fleet:** add declared inventory and resumable canary rollouts ([#536](https://github.com/0xPlayerOne/code-foundry/issues/536)) ([6aa86d4](https://github.com/0xPlayerOne/code-foundry/commit/6aa86d4cd85cdbd4041c70d8c01d8e351e21fc0b))

## [1.12.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.11.0...v1.12.0) (2026-09-09)


### Features

* **cloudflare:** verify candidates before protected version promotion ([#535](https://github.com/0xPlayerOne/code-foundry/issues/535)) ([5dd9afa](https://github.com/0xPlayerOne/code-foundry/commit/5dd9afa8418718823844875b0aedce926b887184))

## [1.11.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.10.1...v1.11.0) (2026-09-09)


### Features

* **validation:** enforce required capabilities, coverage, and task evidence ([#534](https://github.com/0xPlayerOne/code-foundry/issues/534)) ([2e341d9](https://github.com/0xPlayerOne/code-foundry/commit/2e341d94381599f1d78ec1394d42883157b30ea6))

## [1.10.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.10.0...v1.10.1) (2026-09-09)


### Bug Fixes

* **doctor:** honor shared config and correctly identify npm/Yarn lockfiles ([#533](https://github.com/0xPlayerOne/code-foundry/issues/533)) ([6464409](https://github.com/0xPlayerOne/code-foundry/commit/646440907ad3fc47f63e27b9621c8e0025459964))
* **validation:** scan default branch with CodeQL on push ([#540](https://github.com/0xPlayerOne/code-foundry/issues/540)) ([98d8241](https://github.com/0xPlayerOne/code-foundry/commit/98d8241522c78e1b6d3f4f29a44053d33888edba))

## [1.10.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.13...v1.10.0) (2026-09-08)


### Features

* **ci:** enforce draft pull request readiness ([#530](https://github.com/0xPlayerOne/code-foundry/issues/530)) ([fe62147](https://github.com/0xPlayerOne/code-foundry/commit/fe621477a46b49dee69a4c74c482e815a3e60b8d))

## [1.9.13](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.12...v1.9.13) (2026-09-08)


### Bug Fixes

* **cloudflare:** preserve Bun package manager for OpenNext deploys ([#529](https://github.com/0xPlayerOne/code-foundry/issues/529)) ([2f1bc00](https://github.com/0xPlayerOne/code-foundry/commit/2f1bc000ea28e207e4f12cc7abb5c330cb8448b9))

## [1.9.12](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.11...v1.9.12) (2026-09-08)


### Bug Fixes

* **validation:** run available suites for no-CodeQL releases ([805c470](https://github.com/0xPlayerOne/code-foundry/commit/805c470f188ccfe7410bc9b2f02022d50c68f321))

## [1.9.11](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.10...v1.9.11) (2026-09-08)


### Bug Fixes

* **doctor:** support nested Rust crates ([#525](https://github.com/0xPlayerOne/code-foundry/issues/525)) ([0ffc87d](https://github.com/0xPlayerOne/code-foundry/commit/0ffc87d71c5e8069a26814dea2250e93a3e87416))

## [1.9.10](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.9...v1.9.10) (2026-09-08)


### Bug Fixes

* **ci:** keep OpenCode detection visible ([#523](https://github.com/0xPlayerOne/code-foundry/issues/523)) ([5499db8](https://github.com/0xPlayerOne/code-foundry/commit/5499db818f0b06e98f07173893104c655b2b63c1))

## [1.9.9](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.8...v1.9.9) (2026-09-08)


### Bug Fixes

* **sync:** standardize existing release PR titles ([#521](https://github.com/0xPlayerOne/code-foundry/issues/521)) ([76b1c94](https://github.com/0xPlayerOne/code-foundry/commit/76b1c94ee2ddde2a438bbb0cd11515eacbcbdb8d))

## [1.9.8](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.7...v1.9.8) (2026-09-08)


### Bug Fixes

* **docs:** describe full release validation ([#519](https://github.com/0xPlayerOne/code-foundry/issues/519)) ([1c51368](https://github.com/0xPlayerOne/code-foundry/commit/1c513681dcd34d30d16d89505a159061d66e8fdb))

## [1.9.7](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.6...v1.9.7) (2026-09-08)


### Bug Fixes

* **ci:** run full validation on release PRs ([#517](https://github.com/0xPlayerOne/code-foundry/issues/517)) ([01a3555](https://github.com/0xPlayerOne/code-foundry/commit/01a355505d6372dc26e2d917e0e6d566ab25546c))
* **sync:** remove direct topology staging residue ([#515](https://github.com/0xPlayerOne/code-foundry/issues/515)) ([2765e6a](https://github.com/0xPlayerOne/code-foundry/commit/2765e6a6f66137d37f3d65f8eb8311ba28eeafd7))

## [1.9.6](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.5...v1.9.6) (2026-09-08)


### Bug Fixes

* **ci:** finalize direct fleet policy ([#513](https://github.com/0xPlayerOne/code-foundry/issues/513)) ([98c59a7](https://github.com/0xPlayerOne/code-foundry/commit/98c59a713f31d0bc5e3b9893434d89dba3257550))

## [1.9.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.4...v1.9.5) (2026-09-08)


### Bug Fixes

* **docs:** document draft validation behavior ([#511](https://github.com/0xPlayerOne/code-foundry/issues/511)) ([cfa3d9b](https://github.com/0xPlayerOne/code-foundry/commit/cfa3d9b9e7a6c9a4fe5af0dd858552c412d2d542))

## [1.9.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.3...v1.9.4) (2026-09-08)


### Bug Fixes

* **doctor:** accept no-CodeQL validation callers ([#509](https://github.com/0xPlayerOne/code-foundry/issues/509)) ([f447de8](https://github.com/0xPlayerOne/code-foundry/commit/f447de81b8f2e7e59ab6fdbd6b1939635286e2a9))

## [1.9.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.2...v1.9.3) (2026-09-08)


### Bug Fixes

* **ci:** suppress unavailable and draft checks ([#507](https://github.com/0xPlayerOne/code-foundry/issues/507)) ([e0b313a](https://github.com/0xPlayerOne/code-foundry/commit/e0b313ad1e4601ccd14066fb97a4f547400a6eaa))

## [1.9.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.1...v1.9.2) (2026-09-08)


### Bug Fixes

* **sync:** refresh config-aware policies ([#505](https://github.com/0xPlayerOne/code-foundry/issues/505)) ([466150d](https://github.com/0xPlayerOne/code-foundry/commit/466150dcf263187e9cb08be2a2c2fe7ff67ef060))

## [1.9.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.9.0...v1.9.1) (2026-09-08)


### Bug Fixes

* **ci:** restore protected consumer audits ([#503](https://github.com/0xPlayerOne/code-foundry/issues/503)) ([d045cc4](https://github.com/0xPlayerOne/code-foundry/commit/d045cc4a5543d2096e4d6f33c5e74aa40604c887))

## [1.9.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.8.0...v1.9.0) (2026-09-08)


### Features

* **performance:** standardize package audit contracts ([#501](https://github.com/0xPlayerOne/code-foundry/issues/501)) ([ab30081](https://github.com/0xPlayerOne/code-foundry/commit/ab3008120772922a1affd1e5648a99b97b02e455))

## [1.8.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.7.0...v1.8.0) (2026-09-08)


### Features

* **performance:** enforce source budgets ([#499](https://github.com/0xPlayerOne/code-foundry/issues/499)) ([2f65ba1](https://github.com/0xPlayerOne/code-foundry/commit/2f65ba127f8fe186eda5d6bcae77150f13458428))

## [1.7.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.6.1...v1.7.0) (2026-09-08)


### Features

* **release:** standardize generated PR titles ([#497](https://github.com/0xPlayerOne/code-foundry/issues/497)) ([44de0c4](https://github.com/0xPlayerOne/code-foundry/commit/44de0c4f1261a017a0395ddae268c203cccc71b4))

## [1.6.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.6.0...v1.6.1) (2026-09-08)


### Bug Fixes

* **ci:** isolate default-branch security audits ([5ea0914](https://github.com/0xPlayerOne/code-foundry/commit/5ea09146af9995f16d1ab4e9a73f14a13582da36))

## [1.6.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.5.4...v1.6.0) (2026-09-08)


### Features

* **ci:** add shared performance validation ([#492](https://github.com/0xPlayerOne/code-foundry/issues/492)) ([ef12990](https://github.com/0xPlayerOne/code-foundry/commit/ef1299045b6d67e447def93e2096862cde64bbc7))

## [1.5.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.5.3...v1.5.4) (2026-09-08)


### Bug Fixes

* **security:** pin scheduled audit runtime ([#491](https://github.com/0xPlayerOne/code-foundry/issues/491)) ([af25ef6](https://github.com/0xPlayerOne/code-foundry/commit/af25ef6137078809f27c316bdde2a9d025ef34af))

## [1.5.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.5.2...v1.5.3) (2026-09-08)


### Bug Fixes

* **security:** remove cache-capable setup from audits ([#489](https://github.com/0xPlayerOne/code-foundry/issues/489)) ([47bd1d9](https://github.com/0xPlayerOne/code-foundry/commit/47bd1d9495a02dd2abcb2fee82052136b7a3675d))

## [1.5.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.5.1...v1.5.2) (2026-09-08)


### Bug Fixes

* **workflows:** disable security cache writes ([#487](https://github.com/0xPlayerOne/code-foundry/issues/487)) ([f484a9b](https://github.com/0xPlayerOne/code-foundry/commit/f484a9b014b731bc1ae48e4b69a0ac3ae6c07ef6))

## [1.5.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.5.0...v1.5.1) (2026-09-08)


### Bug Fixes

* sync-caller-runtime-pin ([#484](https://github.com/0xPlayerOne/code-foundry/issues/484)) ([e1a216a](https://github.com/0xPlayerOne/code-foundry/commit/e1a216a9dcebd040ef0eacdb20791f360a921908))

## [1.5.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.4.1...v1.5.0) (2026-09-07)


### Features

* **release:** squash release merges, Cloudflare deploy workflow, tooling neutrality ([6a847eb](https://github.com/0xPlayerOne/code-foundry/commit/6a847eb0a3f78dbd343b7b189f32543d621b4b8a))

## [1.4.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.4.0...v1.4.1) (2026-09-07)


### Bug Fixes

* **validation:** run CodeQL on the release tier ([e93c36c](https://github.com/0xPlayerOne/code-foundry/commit/e93c36c4be11611117a13aa88212f16b6129f464))

## [1.4.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.3.2...v1.4.0) (2026-09-07)


### Features

* **sync:** oxfmt-stable config merges, gitignore preservation, and OPENCODE_SECURITY variable override ([455ac37](https://github.com/0xPlayerOne/code-foundry/commit/455ac37635d7e88a0bfe007a98ee12b56bc430dc))

## [1.3.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.3.1...v1.3.2) (2026-09-07)


### Bug Fixes

* preserve consumer-only Oxc config keys across syncs ([#476](https://github.com/0xPlayerOne/code-foundry/issues/476)) ([07aee3a](https://github.com/0xPlayerOne/code-foundry/commit/07aee3aed2aadeccf9740e1966941281e3f031f4))

## [1.3.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.3.0...v1.3.1) (2026-09-07)


### Bug Fixes

* restore job-level OpenCode scanner call; preserve consumer oxlint ignores on sync ([#473](https://github.com/0xPlayerOne/code-foundry/issues/473)) ([171ac3d](https://github.com/0xPlayerOne/code-foundry/commit/171ac3dc57368a6ad1e21d8b439a34cbbe2eca58))

## [1.3.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.2.1...v1.3.0) (2026-09-07)


### Features

* migrate the JavaScript toolchain from ESLint/Prettier to oxlint/oxfmt ([#471](https://github.com/0xPlayerOne/code-foundry/issues/471)) ([8ed872a](https://github.com/0xPlayerOne/code-foundry/commit/8ed872a2c61c6bbac111da645760671c49333dbd))

## [1.2.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.2.0...v1.2.1) (2026-09-06)


### Bug Fixes

* restore pre-matrix CodeQL SARIF category strings ([#468](https://github.com/0xPlayerOne/code-foundry/issues/468)) ([8c51892](https://github.com/0xPlayerOne/code-foundry/commit/8c518921bf3632ba5b8ee4ca757efe3bc302739a))

## [1.2.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.1.1...v1.2.0) (2026-09-06)


### Features

* eliminate skipped checks with unified matrices and an in-gate release check ([#465](https://github.com/0xPlayerOne/code-foundry/issues/465)) ([55c3dca](https://github.com/0xPlayerOne/code-foundry/commit/55c3dca7a7d1460830464ec61f9b083d1350e3dd))

## [1.1.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.1.0...v1.1.1) (2026-09-06)


### Bug Fixes

* keep a static check name for the Rust CodeQL job ([#462](https://github.com/0xPlayerOne/code-foundry/issues/462)) ([c8c4a36](https://github.com/0xPlayerOne/code-foundry/commit/c8c4a364a7f77e404159fbe7c08ee695f78c8b61))

## [1.1.0](https://github.com/0xPlayerOne/code-foundry/compare/v1.0.6...v1.1.0) (2026-09-06)


### Features

* scope per-language checks to detected languages via matrix ([#459](https://github.com/0xPlayerOne/code-foundry/issues/459)) ([71f8985](https://github.com/0xPlayerOne/code-foundry/commit/71f8985b9732d39b7b68df40a4c8cbe5a90175fe))

## [1.0.6](https://github.com/0xPlayerOne/code-foundry/compare/v1.0.5...v1.0.6) (2026-09-06)


### Bug Fixes

* scope dependabot ecosystems to configured languages ([#457](https://github.com/0xPlayerOne/code-foundry/issues/457)) ([2bb9121](https://github.com/0xPlayerOne/code-foundry/commit/2bb91215de662dfa7a38d0c13cc7af1b5b07d798))

## [1.0.5](https://github.com/0xPlayerOne/code-foundry/compare/v1.0.4...v1.0.5) (2026-09-06)


### Bug Fixes

* default runtime-ref inputs to the current runtime release ([#454](https://github.com/0xPlayerOne/code-foundry/issues/454)) ([6d77025](https://github.com/0xPlayerOne/code-foundry/commit/6d77025511ca641e98a17c4eed63a24285a48169))

## [1.0.4](https://github.com/0xPlayerOne/code-foundry/compare/v1.0.3...v1.0.4) (2026-09-06)


### Bug Fixes

* **security:** only save caches on push in security workflow ([fff3e25](https://github.com/0xPlayerOne/code-foundry/commit/fff3e251f13e2f3954a20be8da30d4f274f36eba))

## [1.0.3](https://github.com/0xPlayerOne/code-foundry/compare/v1.0.2...v1.0.3) (2026-09-06)


### Bug Fixes

* **security:** save caches on push events only ([3180b07](https://github.com/0xPlayerOne/code-foundry/commit/3180b07a669b7caa5728be6a07143d60a0c7f6af))

## [1.0.2](https://github.com/0xPlayerOne/code-foundry/compare/v1.0.1...v1.0.2) (2026-09-05)


### Bug Fixes

* **release:** provision bun and corepack before publish install ([32f9b15](https://github.com/0xPlayerOne/code-foundry/commit/32f9b153cdc96cf3c38b379eada41853116e9200))

## [1.0.1](https://github.com/0xPlayerOne/code-foundry/compare/v1.0.0...v1.0.1) (2026-09-05)


### Bug Fixes

* **release:** install dependencies before npm publish ([8e03535](https://github.com/0xPlayerOne/code-foundry/commit/8e0353549c42b982e84c28db94351d752a28d60e))

## [1.0.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.40.3...v1.0.0) (2026-09-05)


### ⚠ BREAKING CHANGES

* automation now reads CODE_FOUNDRY_TOKEN only. Repos still carrying just RELEASE_PLEASE_TOKEN fall back to the short-lived workflow token (manual merges) until they set CODE_FOUNDRY_TOKEN.

### Features

* remove RELEASE_PLEASE_TOKEN fallback in favor of CODE_FOUNDRY_TOKEN ([3f6ba1c](https://github.com/0xPlayerOne/code-foundry/commit/3f6ba1c3cb0db698a7c75485b9e4201720e930d7))

## [0.40.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.40.2...v0.40.3) (2026-09-05)


### Bug Fixes

* **sync:** hold TypeScript toolchain below v7 in consumer dependabot config ([e3c91e1](https://github.com/0xPlayerOne/code-foundry/commit/e3c91e1079bfcd69d174d3ede6d20674eb8fd37b))

## [0.40.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.40.1...v0.40.2) (2026-09-05)


### Bug Fixes

* **validation:** skip eslint fallback without repo setup and ignore overlaid actions ([bb4756c](https://github.com/0xPlayerOne/code-foundry/commit/bb4756cb8a40199f4d0b6bdb47020f0bc7283de1))

## [0.40.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.40.0...v0.40.1) (2026-08-31)


### Bug Fixes

* **validation:** load consumer audit policy ([8d13173](https://github.com/0xPlayerOne/code-foundry/commit/8d13173a36849528335f87a550072e08137f4473))

## [0.40.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.39.4...v0.40.0) (2026-08-31)


### Features

* **validation:** allow audit mode on staging PRs ([0d95123](https://github.com/0xPlayerOne/code-foundry/commit/0d951230b9095d3b875db44ae8287335152eee60))

## [0.39.4](https://github.com/0xPlayerOne/code-foundry/compare/v0.39.3...v0.39.4) (2026-08-29)


### Bug Fixes

* **security:** pin authoritative scan resealing ([6885fea](https://github.com/0xPlayerOne/code-foundry/commit/6885fea2848ec13ae6a8fc6c3f378c7b98a46a9f))

## [0.39.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.39.2...v0.39.3) (2026-08-29)


### Bug Fixes

* **security:** pin scanner target normalization ([f03ddb0](https://github.com/0xPlayerOne/code-foundry/commit/f03ddb07d9bc6c06d9a94962f475ec157e5d194e))

## [0.39.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.39.1...v0.39.2) (2026-08-29)


### Bug Fixes

* **release:** qualify promotion PR head filters ([75a0985](https://github.com/0xPlayerOne/code-foundry/commit/75a09856d764aafc1cd301ae68121e187c43e2d1))

## [0.39.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.39.0...v0.39.1) (2026-08-29)


### Bug Fixes

* **release:** build exact-tree reconciliation heads ([33b0151](https://github.com/0xPlayerOne/code-foundry/commit/33b015102f07ca03ffb677fe4b9f5e67bbf9a485))

## [0.39.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.38.2...v0.39.0) (2026-08-29)


### Features

* code-foundry 0.38.3 — direct workflow default, muse spark model, opencode_security_model override ([436da59](https://github.com/0xPlayerOne/code-foundry/commit/436da5947098039642cb961987e962cd88960db8))


### Bug Fixes

* draft-pr base main for direct workflow (staging deleted) ([b1c063f](https://github.com/0xPlayerOne/code-foundry/commit/b1c063fa8e967800b85ffb9ae42df5d62e9a4e1e))

## [0.38.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.38.1...v0.38.2) (2026-08-29)


### Bug Fixes

* **release:** preserve promotion release semantics ([#418](https://github.com/0xPlayerOne/code-foundry/issues/418)) ([b1702a7](https://github.com/0xPlayerOne/code-foundry/commit/b1702a756cc6d7297f98b529b0bca178a1cdc3d1))

## [0.38.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.38.0...v0.38.1) (2026-08-29)


### Bug Fixes

* **release:** avoid unsafe history-only reconciliation PRs ([#412](https://github.com/0xPlayerOne/code-foundry/issues/412)) ([941f08b](https://github.com/0xPlayerOne/code-foundry/commit/941f08ba7e830ec3ab0ae9c6b937e488c621b95e))

## [0.38.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.37.5...v0.38.0) (2026-08-24)


### Features

* **ci:** add reversible billing pause ([#402](https://github.com/0xPlayerOne/code-foundry/issues/402)) ([aa17b11](https://github.com/0xPlayerOne/code-foundry/commit/aa17b11037dccced17dd1173d9d788ac83ba50b5))


### Bug Fixes

* **ci:** guard every workflow during billing pause ([#405](https://github.com/0xPlayerOne/code-foundry/issues/405)) ([fc3930f](https://github.com/0xPlayerOne/code-foundry/commit/fc3930fcb50e9182bb0f5e97ea523a6805f3fa95))
* **release:** allow explicit release while CI is paused ([#407](https://github.com/0xPlayerOne/code-foundry/issues/407)) ([3d31cf1](https://github.com/0xPlayerOne/code-foundry/commit/3d31cf154255225ecdd9bca94f8620ad8c2b3473))

## [0.37.5](https://github.com/0xPlayerOne/code-foundry/compare/v0.37.4...v0.37.5) (2026-08-23)


### Bug Fixes

* **sync:** omit Cargo Dependabot outside Rust repos ([#398](https://github.com/0xPlayerOne/code-foundry/issues/398)) ([395c4f3](https://github.com/0xPlayerOne/code-foundry/commit/395c4f34887bbb3e9f67378325b70c21d467adf0))

## [0.37.4](https://github.com/0xPlayerOne/code-foundry/compare/v0.37.3...v0.37.4) (2026-08-23)


### Bug Fixes

* release-workspace-state ([#395](https://github.com/0xPlayerOne/code-foundry/issues/395)) ([a708bc0](https://github.com/0xPlayerOne/code-foundry/commit/a708bc07272b9751b22a457771cc386601bbe3d8))

## [0.37.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.37.2...v0.37.3) (2026-08-23)


### Bug Fixes

* release-required-check-discovery ([#392](https://github.com/0xPlayerOne/code-foundry/issues/392)) ([d086cb5](https://github.com/0xPlayerOne/code-foundry/commit/d086cb5b6d1dc25eb28b6551ae56467887637296))

## [0.37.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.37.1...v0.37.2) (2026-08-23)


### Bug Fixes

* **ci:** stabilize runners and release reconciliation ([#387](https://github.com/0xPlayerOne/code-foundry/issues/387)) ([ea2c503](https://github.com/0xPlayerOne/code-foundry/commit/ea2c503cb6ea9b944ffa5b70ff7fbfc3d56d3a10))

## [0.37.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.37.0...v0.37.1) (2026-08-08)


### Bug Fixes

* **sync:** prettier-canonical CONTRIBUTING.md tables for both topologies ([af9137b](https://github.com/0xPlayerOne/code-foundry/commit/af9137bc788853ed97c4c17aef9848b7f9d15fbf))

## [0.37.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.36.2...v0.37.0) (2026-08-07)


### Features

* **agents:** add explicit merge-workflow guidance ([a74c0ce](https://github.com/0xPlayerOne/code-foundry/commit/a74c0ce61c8dc53795a645ab5f2062ded732e3a5))

## [0.36.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.36.1...v0.36.2) (2026-08-07)


### Bug Fixes

* **sync:** prettier-canonical dependabot ignore quotes ([491e06a](https://github.com/0xPlayerOne/code-foundry/commit/491e06ade14531eb02f1d7aa729cee3b1acdf78b))

## [0.36.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.36.0...v0.36.1) (2026-08-07)


### Bug Fixes

* **sync:** prettier-canonical direct doc tables + dependabot ignore for runtime pins ([f4286b6](https://github.com/0xPlayerOne/code-foundry/commit/f4286b62ac06145b250d02ede9421f36df72a344))

## [0.36.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.35.0...v0.36.0) (2026-08-07)


### Features

* make staging-release opt-in and direct-to-main the default ([#370](https://github.com/0xPlayerOne/code-foundry/issues/370)) ([7c66507](https://github.com/0xPlayerOne/code-foundry/commit/7c665071769f0b0332e2f47929ee0c19bbfd5af3))

## [0.35.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.14...v0.35.0) (2026-08-04)


### Features

* support Apache 2.0 license sync ([538e7e4](https://github.com/0xPlayerOne/code-foundry/commit/538e7e4e85f9ee8c0af3e319f0440fc78e14dae9))


### Bug Fixes

* validate license policy before sync ([5baffa8](https://github.com/0xPlayerOne/code-foundry/commit/5baffa80c59f907fbf27974b43dfa4e063842d71))

## [0.34.14](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.13...v0.34.14) (2026-08-03)


### Bug Fixes

* **reconcile:** ignore historical paths absent from final tree ([#362](https://github.com/0xPlayerOne/code-foundry/issues/362)) ([8b8a123](https://github.com/0xPlayerOne/code-foundry/commit/8b8a123a1a7ea23a789c491414d3c9ea235a3d72))

## [0.34.13](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.12...v0.34.13) (2026-08-03)


### Bug Fixes

* **reconcile:** classify patch-equivalent trees consistently ([#360](https://github.com/0xPlayerOne/code-foundry/issues/360)) ([c95f1bd](https://github.com/0xPlayerOne/code-foundry/commit/c95f1bdeaa69fc5fbcd42821bc633edbbd31de49))
* **release:** use rebase for release PRs ([#358](https://github.com/0xPlayerOne/code-foundry/issues/358)) ([3b2b2f5](https://github.com/0xPlayerOne/code-foundry/commit/3b2b2f5cee15e3f61a1688e5b3ef0847a6eb8c55))

## [0.34.12](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.11...v0.34.12) (2026-08-02)


### Bug Fixes

* **reconcile:** classify final tree deltas ([#353](https://github.com/0xPlayerOne/code-foundry/issues/353)) ([18d23e4](https://github.com/0xPlayerOne/code-foundry/commit/18d23e4847ffbcfc274bc11c80244ecac64395ed))

## [0.34.11](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.10...v0.34.11) (2026-08-02)


### Bug Fixes

* **draft-pr:** fall back to workflow token ([#350](https://github.com/0xPlayerOne/code-foundry/issues/350)) ([aef07db](https://github.com/0xPlayerOne/code-foundry/commit/aef07db6945badd7d7b3526b5490b1512ac1a468))

## [0.34.10](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.9...v0.34.10) (2026-08-02)


### Bug Fixes

* **release:** validate automation token before Release Please ([654094f](https://github.com/0xPlayerOne/code-foundry/commit/654094f452a4a6351de247aa82bf2448d7ea79c6))

## [0.34.9](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.8...v0.34.9) (2026-08-02)


### Bug Fixes

* **ci:** fall back to github token for promotion ([37ff019](https://github.com/0xPlayerOne/code-foundry/commit/37ff019e95a9024338c05fec7579476bd5cf0b3f))

## [0.34.8](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.7...v0.34.8) (2026-08-02)


### Bug Fixes

* **ci:** create promotion PRs through REST ([c123e21](https://github.com/0xPlayerOne/code-foundry/commit/c123e21e868de685a91de228ca57cf6614767bb7))

## [0.34.7](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.6...v0.34.7) (2026-08-02)


### Bug Fixes

* **release:** authenticate partial clone comparisons ([172dfbe](https://github.com/0xPlayerOne/code-foundry/commit/172dfbef53ab1a9eee44cf68f648889ae99b93b1))

## [0.34.6](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.5...v0.34.6) (2026-08-02)


### Bug Fixes

* **sync:** keep prettier ignores idempotent ([5db5307](https://github.com/0xPlayerOne/code-foundry/commit/5db53072fded27a57cca3cedf7c40527cd238507))

## [0.34.5](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.4...v0.34.5) (2026-08-02)


### Bug Fixes

* **release:** reconcile protected staging branches ([fa18bfb](https://github.com/0xPlayerOne/code-foundry/commit/fa18bfbb90aaed5c78ff70dbb3dc17d5633e7e5f))

## [0.34.4](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.3...v0.34.4) (2026-08-02)


### Bug Fixes

* split native test suites by category ([93c9ede](https://github.com/0xPlayerOne/code-foundry/commit/93c9ede6e202a790befe1ee0e57633e3d01dc428))

## [0.34.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.2...v0.34.3) (2026-08-02)


### Bug Fixes

* **release:** reconcile only after creating a release ([#317](https://github.com/0xPlayerOne/code-foundry/issues/317)) ([#318](https://github.com/0xPlayerOne/code-foundry/issues/318)) ([6f2b00c](https://github.com/0xPlayerOne/code-foundry/commit/6f2b00c5f3fe27e56b448671902bf6f5e33cca1f))

## [0.34.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.1...v0.34.2) (2026-08-01)


### Bug Fixes

* **release:** make mergeability poll executable ([#314](https://github.com/0xPlayerOne/code-foundry/issues/314)) ([66161ab](https://github.com/0xPlayerOne/code-foundry/commit/66161abe151f6fa7ec09844aa6fa5dab83b37de6))

## [0.34.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.34.0...v0.34.1) (2026-08-01)


### Bug Fixes

* **release:** wait for PR mergeability before guarded auto-merge ([#311](https://github.com/0xPlayerOne/code-foundry/issues/311)) ([e9be192](https://github.com/0xPlayerOne/code-foundry/commit/e9be192e6b42020f327d42d928f2c6a835358e59))

## [0.34.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.33.0...v0.34.0) (2026-08-01)


### Features

* **release:** classify reconcile push failures and log sanitized details ([#307](https://github.com/0xPlayerOne/code-foundry/issues/307)) ([0651fca](https://github.com/0xPlayerOne/code-foundry/commit/0651fca3eb4f11eeb21b91462397eef865eee7cc))


### Bug Fixes

* **release:** include ssh executable in reconcile transport ([#308](https://github.com/0xPlayerOne/code-foundry/issues/308)) ([49713ed](https://github.com/0xPlayerOne/code-foundry/commit/49713edeaf5262a0ed872aa6d3fdf55927b6e1c5))
* **release:** keep reconcile fetch over HTTPS ([#305](https://github.com/0xPlayerOne/code-foundry/issues/305)) ([022afad](https://github.com/0xPlayerOne/code-foundry/commit/022afade430a00b9656dcfa50af3056bb27a54e3))

## [0.33.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.32.4...v0.33.0) (2026-08-01)


### Features

* add tiered validation workflow ([#301](https://github.com/0xPlayerOne/code-foundry/issues/301)) ([dd3015e](https://github.com/0xPlayerOne/code-foundry/commit/dd3015ea22ab94b2ed3d55f6e900a04f3e968aeb))


### Bug Fixes

* preserve regex escape in test assertion ([#303](https://github.com/0xPlayerOne/code-foundry/issues/303)) ([0a3c56f](https://github.com/0xPlayerOne/code-foundry/commit/0a3c56f5318baa8002b1079687797702f2c06383))

## [0.32.4](https://github.com/0xPlayerOne/code-foundry/compare/v0.32.3...v0.32.4) (2026-08-01)


### Bug Fixes

* **sync:** never leak runtime release-type into consumer configs ([b7c51f3](https://github.com/0xPlayerOne/code-foundry/commit/b7c51f3e465e048be933292e0db9ca08d5420c9a))
* **sync:** quote collection-like config values so prettier accepts them ([b0d4fea](https://github.com/0xPlayerOne/code-foundry/commit/b0d4fea815b6417de23cf577cba525e2017004dc))
* **sync:** satisfy JSDoc type-check for baseline merge ([ce54339](https://github.com/0xPlayerOne/code-foundry/commit/ce54339b2092722e4d0d4e43afdb7ab5bacd2bc1))

## [0.32.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.32.2...v0.32.3) (2026-07-31)


### Bug Fixes

* **release:** no-op when staging already points at main's commit ([a47180a](https://github.com/0xPlayerOne/code-foundry/commit/a47180a16ae8b9fd66548aba284939b3cdfaeba8))
* **release:** squash Release Please PRs for release-please compatibility ([41c808b](https://github.com/0xPlayerOne/code-foundry/commit/41c808b8c2502ca78e271cb6702334daf90169da))

## [0.32.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.32.1...v0.32.2) (2026-07-31)


### Bug Fixes

* **release:** mirror staging onto main and require rebase merges on main ([31ab9b1](https://github.com/0xPlayerOne/code-foundry/commit/31ab9b125e66ae35f7d2a2c6893d0a3aec5d4560))
* **release:** synchronize staging with a linear commit instead of a blocked fast-forward ([b808dff](https://github.com/0xPlayerOne/code-foundry/commit/b808dffeae38ec8211f8f0dee79e19d60f70b708))

## [0.32.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.32.0...v0.32.1) (2026-07-31)


### Bug Fixes

* **ci:** key runtime concurrency by event so promotion PRs do not cancel push checks ([5a8d8fd](https://github.com/0xPlayerOne/code-foundry/commit/5a8d8fd80e62feabc887869e07219a77f2c46c1a))
* **release:** bootstrap release-please manifest during sync ([98c7e5d](https://github.com/0xPlayerOne/code-foundry/commit/98c7e5d9341eedf22d49611f19825a5ef8d6d596))
* **release:** satisfy JSDoc type-check for manifest bootstrap ([02ddb45](https://github.com/0xPlayerOne/code-foundry/commit/02ddb459405ee9d54c91afdc3cf5602790a4c2b4))
* **release:** squash release PRs so staging can fast-forward after releases ([5d9a788](https://github.com/0xPlayerOne/code-foundry/commit/5d9a78843fde4ce764237eacfde9b1720d15696e))

## [0.32.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.18...v0.32.0) (2026-07-31)


### Features

* improve draft PR titles from branch conventions ([#290](https://github.com/0xPlayerOne/code-foundry/issues/290)) ([7b215db](https://github.com/0xPlayerOne/code-foundry/commit/7b215db961347dfdb74241fc2c3489d390b34533))

## [0.31.18](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.17...v0.31.18) (2026-07-30)


### Bug Fixes

* **codeql:** keep generated config in workspace ([9ca8f3b](https://github.com/0xPlayerOne/code-foundry/commit/9ca8f3b958e40209727f305bd0c0856f4820e1b6))

## [0.31.17](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.16...v0.31.17) (2026-07-30)


### Bug Fixes

* **sync:** preserve repository release policy ([8a8291b](https://github.com/0xPlayerOne/code-foundry/commit/8a8291b940bcc777e4aa9a426e56235b031fd002))

## [0.31.16](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.15...v0.31.16) (2026-07-30)


### Bug Fixes

* **release:** avoid duplicate release PR checks ([42d7354](https://github.com/0xPlayerOne/code-foundry/commit/42d735404cd7b77d5a30a03a4fb8856096e931b0))
* **workflows:** validate main promotion PRs ([4f41f90](https://github.com/0xPlayerOne/code-foundry/commit/4f41f90a3e4a5eec8e80d46c21083c1380655341))

## [0.31.15](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.14...v0.31.15) (2026-07-30)


### Bug Fixes

* **release:** suppress release-only promotion loops ([fb35a6f](https://github.com/0xPlayerOne/code-foundry/commit/fb35a6f6e03a8ab4da65eeaeeeec579389b508b3))

## [0.31.14](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.13...v0.31.14) (2026-07-30)


### Bug Fixes

* **codeql:** make Rust parallelism safe and configurable ([545454f](https://github.com/0xPlayerOne/code-foundry/commit/545454fa42a8bb4e6970ff858af186f1cba09900))

## [0.31.13](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.12...v0.31.13) (2026-07-30)


### Bug Fixes

* **runtime:** pin template defaults to v0.31.12 ([f84b62d](https://github.com/0xPlayerOne/code-foundry/commit/f84b62d50955c623b9bc67e981645d9c0fcb2bcd))

## [0.31.12](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.11...v0.31.12) (2026-07-30)


### Bug Fixes

* **package:** include ruff baseline ([645f63e](https://github.com/0xPlayerOne/code-foundry/commit/645f63e9e66d67338345bb3eb14949543f97f89b))

## [0.31.11](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.10...v0.31.11) (2026-07-30)


### Bug Fixes

* **package:** include prettier ignore baseline ([4cf91e1](https://github.com/0xPlayerOne/code-foundry/commit/4cf91e1d0ec6b53e3751469937b44f903ef09466))

## [0.31.10](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.9...v0.31.10) (2026-07-30)


### Bug Fixes

* **opencode:** avoid duplicate self checks ([71b1201](https://github.com/0xPlayerOne/code-foundry/commit/71b1201baf58624401676b99fa257780b1eb1abc))

## [0.31.9](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.8...v0.31.9) (2026-07-30)


### Bug Fixes

* **doctor:** deduplicate required check contexts ([f244494](https://github.com/0xPlayerOne/code-foundry/commit/f24449448f177c99978fe216b92385909f275d89))

## [0.31.8](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.7...v0.31.8) (2026-07-30)


### Bug Fixes

* **runtime:** pin self workflows to v0.31.7 ([565b5bc](https://github.com/0xPlayerOne/code-foundry/commit/565b5bcc2b8f4ade8b3addc02f72c96a42308325))

## [0.31.7](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.6...v0.31.7) (2026-07-30)


### Bug Fixes

* **ci:** remove duplicate promotion checks ([b210b7f](https://github.com/0xPlayerOne/code-foundry/commit/b210b7f0aa5bdb6cb7e121cc751b6f618512ebf3))

## [0.31.6](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.5...v0.31.6) (2026-07-30)


### Bug Fixes

* **release:** skip identical promotion trees ([d8242b9](https://github.com/0xPlayerOne/code-foundry/commit/d8242b9897c9210a2534712fedb12d2258573686))

## [0.31.5](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.4...v0.31.5) (2026-07-30)


### Bug Fixes

* **ci:** isolate reusable workflow concurrency ([330a939](https://github.com/0xPlayerOne/code-foundry/commit/330a9396390aef11a482bf370dbbbee22151759e))
* **ci:** use stable workflow concurrency keys ([a7eca35](https://github.com/0xPlayerOne/code-foundry/commit/a7eca35836f24f9fb240234b999462f95fa4e7da))
* **ci:** validate main promotion pull requests ([00377bb](https://github.com/0xPlayerOne/code-foundry/commit/00377bb6e54288e296245efa1466e8e61477f25a))
* **release:** allow manual promotion validation ([aaa453f](https://github.com/0xPlayerOne/code-foundry/commit/aaa453f3bc63c4e256352f094468f983dad236a9))
* **release:** promote staging runtime safeguards ([e53df8c](https://github.com/0xPlayerOne/code-foundry/commit/e53df8cca59e59a8ffd7aad3f05effc915ba2196))

## [0.31.4](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.3...v0.31.4) (2026-07-29)


### Bug Fixes

* harden fleet pins and github doctor ([c6efa7a](https://github.com/0xPlayerOne/code-foundry/commit/c6efa7a436308959950d958c5897574193cd763b))

## [0.31.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.2...v0.31.3) (2026-07-29)


### Bug Fixes

* **ci:** isolate runtime from consumer tooling ([9bb07da](https://github.com/0xPlayerOne/code-foundry/commit/9bb07daa383a3ec89a57c6279546f1d8d4483457))
* **ci:** keep runtime out of project tooling ([0aec04a](https://github.com/0xPlayerOne/code-foundry/commit/0aec04a01f6378f165b83dbedde670ddee61657e))

## [0.31.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.1...v0.31.2) (2026-07-29)


### Bug Fixes

* **release:** treat identical branch trees as aligned ([32b739e](https://github.com/0xPlayerOne/code-foundry/commit/32b739e8e663dca05fd89005b26c6457ec265c1c))

## [0.31.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.31.0...v0.31.1) (2026-07-29)


### Bug Fixes

* **release:** build clean staging sync branches ([03a7c19](https://github.com/0xPlayerOne/code-foundry/commit/03a7c191d7a5a6b95cce639e6ed9201b374f1010))

## [0.31.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.30.4...v0.31.0) (2026-07-29)


### Features

* **release:** open safe staging sync PRs ([6adb1dc](https://github.com/0xPlayerOne/code-foundry/commit/6adb1dc63966e5bfe70deb3ccd3c3aa5e93ccfad))


### Bug Fixes

* **release:** compare promoted branch tips ([081666b](https://github.com/0xPlayerOne/code-foundry/commit/081666b774418ab333d34eb9a3ca2a8c3bd60c78))

## [0.30.4](https://github.com/0xPlayerOne/code-foundry/compare/v0.30.3...v0.30.4) (2026-07-29)


### Bug Fixes

* **ci:** isolate runtime from consumer tooling ([32fe3ee](https://github.com/0xPlayerOne/code-foundry/commit/32fe3eea20ddad6086c1cfcacff6e7cb90606da0))
* **self-ci:** test the checked-out runtime revision ([93973ba](https://github.com/0xPlayerOne/code-foundry/commit/93973bac19da7d250e3ccda4d4c79b1b0033008b))

## [0.30.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.30.2...v0.30.3) (2026-07-29)


### Bug Fixes

* **fleet:** branch upgrades from remote staging ([58d4389](https://github.com/0xPlayerOne/code-foundry/commit/58d43890436789ec5289e0aaeea71dea0375a140))

## [0.30.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.30.1...v0.30.2) (2026-07-29)


### Bug Fixes

* **fleet:** support explicit repository exclusions ([2c3a641](https://github.com/0xPlayerOne/code-foundry/commit/2c3a641814de392457f94f3581f01e5b625056ee))

## [0.30.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.30.0...v0.30.1) (2026-07-29)


### Bug Fixes

* **release:** retry generated PR discovery ([dba7233](https://github.com/0xPlayerOne/code-foundry/commit/dba72337a04e73a2436d417b9e6f68d67bf54f83))
* **sync:** include Python formatter baseline ([c7ce208](https://github.com/0xPlayerOne/code-foundry/commit/c7ce2084dcc7a7a3372056b879f435276e31aaa0))

## [0.30.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.29.0...v0.30.0) (2026-07-29)


### Features

* **ci:** recommend stack-aware runners ([83df327](https://github.com/0xPlayerOne/code-foundry/commit/83df32777344898651d71af28496202337ae6788))
* **doctor:** validate GitHub release configuration ([877525c](https://github.com/0xPlayerOne/code-foundry/commit/877525c11f6713b235aa3945dd98d017bef5732e))
* **fleet:** add isolated repository upgrades ([76d1765](https://github.com/0xPlayerOne/code-foundry/commit/76d176593ea025a2090bd62f21b275d261d3a9d5))
* **release:** add exactly-once post-release hooks ([f4ffa13](https://github.com/0xPlayerOne/code-foundry/commit/f4ffa136ef972665fe269b6685f9c4b840fc95a9))
* **release:** add non-destructive recovery planning ([6c45592](https://github.com/0xPlayerOne/code-foundry/commit/6c45592358d9ceb0335acc6584ac565971433737))
* **security:** add opt-in OpenCode release scan ([34512c1](https://github.com/0xPlayerOne/code-foundry/commit/34512c1507519d2b37a9bd665243490fa888beb9))
* **sync:** formalize custom workflow overlays ([ee540f9](https://github.com/0xPlayerOne/code-foundry/commit/ee540f9a80c0b128100e795471042fc12aefc226))


### Bug Fixes

* **release:** grant post-release dispatch permission ([c18a52d](https://github.com/0xPlayerOne/code-foundry/commit/c18a52dff2ac76e648eeb9fa1f92fab8a01dafec))

## [0.29.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.28.0...v0.29.0) (2026-07-29)


### Features

* **release:** detect mixed-language release manifests ([f2daa61](https://github.com/0xPlayerOne/code-foundry/commit/f2daa616f2d8cfd2883f960823e862768454fbd6))

## [0.28.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.18...v0.28.0) (2026-07-29)


### Features

* **release:** reconcile staging after release metadata ([4de1ad6](https://github.com/0xPlayerOne/code-foundry/commit/4de1ad64bd9276344368934ab555e6cb31a90784))

## [0.27.18](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.17...v0.27.18) (2026-07-29)


### Bug Fixes

* **release:** degrade gracefully without release token ([69ac43a](https://github.com/0xPlayerOne/code-foundry/commit/69ac43acfa2813495b8da0535942afbbedae3017))

## [0.27.17](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.16...v0.27.17) (2026-07-29)


### Bug Fixes

* **release:** auto-merge generated version PRs ([3032cfc](https://github.com/0xPlayerOne/code-foundry/commit/3032cfc458e4508ad637354ee98447c544a5a1d4))

## [0.27.16](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.15...v0.27.16) (2026-07-29)

### Bug Fixes

- **release:** honor manifest configuration ([2beb320](https://github.com/0xPlayerOne/code-foundry/commit/2beb32053e5b86319a3c44377e4cbe2f20592507))
- **release:** pass committed manifest config ([39ef227](https://github.com/0xPlayerOne/code-foundry/commit/39ef227828d9c7903e9d08cfcd0dd755f41a7c78))

## [0.27.15](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.14...v0.27.15) (2026-07-29)

### Bug Fixes

- **ci:** remove stale CodeQL change detection ([897d749](https://github.com/0xPlayerOne/code-foundry/commit/897d749d296c02751fda764b9fa069e32208182b))

## [0.27.14](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.13...v0.27.14) (2026-07-29)

### Bug Fixes

- **codeql:** skip unavailable analyzers ([9ddf8e3](https://github.com/0xPlayerOne/code-foundry/commit/9ddf8e30dab4da2ba1f6bb20dd3503e56ab1b880))
- **draft-pr:** pass repository explicitly ([6fbf289](https://github.com/0xPlayerOne/code-foundry/commit/6fbf289649ce2097e42b156cf2db0c39fb8ceee1))
- **draft-pr:** use explicit repository for lookups ([e498d6e](https://github.com/0xPlayerOne/code-foundry/commit/e498d6e125099e2437041112e1b3442a7ebea389))

## [0.27.13](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.12...v0.27.13) (2026-07-29)

### Bug Fixes

- **sync:** package the gitignore template ([e65c63d](https://github.com/0xPlayerOne/code-foundry/commit/e65c63dcb09a623d5ce0b55f734bbe73719c72f2))

## [0.27.12](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.11...v0.27.12) (2026-07-29)

### Bug Fixes

- **security:** skip irrelevant dependency audits ([cc206d4](https://github.com/0xPlayerOne/code-foundry/commit/cc206d4dea5311684b79ef3a04669aa7ce74421a))

## [0.27.11](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.10...v0.27.11) (2026-07-29)

### Bug Fixes

- **ci:** isolate reusable workflow concurrency ([ddfc3a6](https://github.com/0xPlayerOne/code-foundry/commit/ddfc3a6b8860629a12494ffd8ef273dfb2c354b4))
- **workflows:** clarify Code Foundry job hierarchy ([124327e](https://github.com/0xPlayerOne/code-foundry/commit/124327ec3f8f5907eca478580a62b7485e0cfd98))

## [0.27.10](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.9...v0.27.10) (2026-07-28)

### Bug Fixes

- **codeql:** make analyzer checks protection-safe ([5ab240e](https://github.com/0xPlayerOne/code-foundry/commit/5ab240e6ce62c2d87acf92f8776a107cffefd860))

## [0.27.9](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.8...v0.27.9) (2026-07-28)

### Bug Fixes

- **ci:** hoist Bun workspace dependencies ([f480ad6](https://github.com/0xPlayerOne/code-foundry/commit/f480ad671cf12435f632d9397dbc8f72d7a2e8fe))

## [0.27.8](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.7...v0.27.8) (2026-07-28)

### Bug Fixes

- **ci:** run required Bun postinstall setup safely ([0302604](https://github.com/0xPlayerOne/code-foundry/commit/0302604f877bedbef8d3ab06794ffd9599fb774c))

## [0.27.7](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.6...v0.27.7) (2026-07-28)

### Bug Fixes

- **ci:** avoid recursive Bun install lifecycle scripts ([780e90d](https://github.com/0xPlayerOne/code-foundry/commit/780e90dcbc4a93005091465594cb57d9d2154003))

## [0.27.6](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.5...v0.27.6) (2026-07-28)

### Bug Fixes

- **ci:** force complete Bun workspace installs ([1d391b8](https://github.com/0xPlayerOne/code-foundry/commit/1d391b8e481acd91d7ae293cdbbfc090a891dc47))

## [0.27.5](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.4...v0.27.5) (2026-07-28)

### Bug Fixes

- **ci:** install Rust formatting and lint components ([16da3fc](https://github.com/0xPlayerOne/code-foundry/commit/16da3fc416e64b2c5c62d2f3a7feaa270134c1a2))
- **test:** skip absent Python integration suites ([ee932ce](https://github.com/0xPlayerOne/code-foundry/commit/ee932cea048dc94175f395ac49ca65ed9dbb466f))

## [0.27.4](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.3...v0.27.4) (2026-07-28)

### Bug Fixes

- **runtime:** resolve Python tools from virtualenv ([788b1ae](https://github.com/0xPlayerOne/code-foundry/commit/788b1ae438451ee57ce55a8669d2710cb8755fcf))

## [0.27.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.2...v0.27.3) (2026-07-28)

### Bug Fixes

- **ci:** auto-detect format tooling ([2be5228](https://github.com/0xPlayerOne/code-foundry/commit/2be522821b5d3f93b92ca5e2c4b20df345396fc3))

## [0.27.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.1...v0.27.2) (2026-07-28)

### Bug Fixes

- **runtime:** harden dependency setup and audits ([f3c4f85](https://github.com/0xPlayerOne/code-foundry/commit/f3c4f85263232e5023e7e6b3ae50ad2c27f3a47a))

## [0.27.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.27.0...v0.27.1) (2026-07-28)

### Bug Fixes

- **ci:** cover framework and native test prerequisites ([53b8209](https://github.com/0xPlayerOne/code-foundry/commit/53b8209104cf52972e867eba65fed46d0b8f57bb))
- **ci:** install project format and Python tooling ([13fb972](https://github.com/0xPlayerOne/code-foundry/commit/13fb972e774e26c2d5794421a17c4ac685a28b0c))

## [0.27.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.26.0...v0.27.0) (2026-07-28)

### Features

- add typed javascript cli checks ([2d9464b](https://github.com/0xPlayerOne/code-foundry/commit/2d9464bcbef8aa51607cdf52a6a60e3fc1bdb054))
- make mise an optional toolchain ([e62f023](https://github.com/0xPlayerOne/code-foundry/commit/e62f0238f4ddc2d1b0f89e0f2b23bca3679b934e))
- make paid github security checks opt-in ([bbfe899](https://github.com/0xPlayerOne/code-foundry/commit/bbfe8993d88a8415129ce29bfa5d2181807232ba))
- skip irrelevant language configuration ([39a0003](https://github.com/0xPlayerOne/code-foundry/commit/39a00037ba92152926e7a89759f3255d86a4f26e))
- standardize optional github security policies ([2cf6bc3](https://github.com/0xPlayerOne/code-foundry/commit/2cf6bc3af161ed8757a03447aab16f3e7ea310d7))

### Bug Fixes

- include runtime libraries in every workflow job ([ce94cd9](https://github.com/0xPlayerOne/code-foundry/commit/ce94cd96a32eff54048712e1bf4b2d34a868ba2e))
- include runtime libraries in workflow checkout ([4b2c252](https://github.com/0xPlayerOne/code-foundry/commit/4b2c2527c37c82b498c2b3457df5dd52ef7c694f))
- migrate stale managed docs during sync ([380bab1](https://github.com/0xPlayerOne/code-foundry/commit/380bab1334c9125f97bf333cc29c796e1a16d57d))
- preserve authored notice files ([342e666](https://github.com/0xPlayerOne/code-foundry/commit/342e666f4e218e094180f10ecdc5a24b85a27b28))
- preserve repository notice attribution ([7d43911](https://github.com/0xPlayerOne/code-foundry/commit/7d439117ec89882d8d06895528d94ed717ade471))
- use pinned bun lockfile format ([0f75faf](https://github.com/0xPlayerOne/code-foundry/commit/0f75faf2c7614cc7055cbb4f26a01b3cf1639f85))

## [0.26.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.25.0...v0.26.0) (2026-07-28)

### Features

- default new repositories to gplv3 ([e200135](https://github.com/0xPlayerOne/code-foundry/commit/e200135939779693eb73a64aaf3587eccdc36ffc))

## [0.25.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.24.1...v0.25.0) (2026-07-28)

### Features

- simplify reusable workflow layout ([293b2a8](https://github.com/0xPlayerOne/code-foundry/commit/293b2a877500853778f311763cd4176e86f0b4f8))

### Bug Fixes

- use local self workflow references ([31ea5a5](https://github.com/0xPlayerOne/code-foundry/commit/31ea5a5a621039afd8e19febe9d2a9f814c9d6fa))

## [0.24.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.24.0...v0.24.1) (2026-07-28)

### Bug Fixes

- remove obsolete consumer helper ([4fcf85b](https://github.com/0xPlayerOne/code-foundry/commit/4fcf85b2c452e08aab47ec1fb6e00cdce5523cff))

## [0.24.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.23.1...v0.24.0) (2026-07-28)

### Features

- minimize consumer footprint ([2b29d2e](https://github.com/0xPlayerOne/code-foundry/commit/2b29d2e09072492c8ee8fc642d0477f416805cf2))

## [0.23.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.23.0...v0.23.1) (2026-07-28)

### Bug Fixes

- support repositories without package managers ([a126945](https://github.com/0xPlayerOne/code-foundry/commit/a126945d259875763ce89ddb3c0dbc182b74bb76))

## [0.23.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.22.2...v0.23.0) (2026-07-28)

### Features

- simplify initialization and synchronization ([9f4643e](https://github.com/0xPlayerOne/code-foundry/commit/9f4643e854a262eb923a4fe84ddb986c3f1bdf77))

## [0.22.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.22.1...v0.22.2) (2026-07-28)

### Bug Fixes

- remove legacy config after migration ([839a4bd](https://github.com/0xPlayerOne/code-foundry/commit/839a4bd7d818633f1aef201b4a2b3292218563f4))

## [0.22.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.22.0...v0.22.1) (2026-07-28)

### Bug Fixes

- pin callers to the canonical runtime ([321b93f](https://github.com/0xPlayerOne/code-foundry/commit/321b93fff2089ee61fa41f968ee584af864692b2))

## [0.22.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.21.2...v0.22.0) (2026-07-28)

### Features

- centralize repository configuration ([e1b4ef1](https://github.com/0xPlayerOne/code-foundry/commit/e1b4ef19ab1ecc899c06331cbfd3477062a73549))

### Bug Fixes

- bridge legacy runtime configuration ([d906b0d](https://github.com/0xPlayerOne/code-foundry/commit/d906b0d8f0bc65d2697ababbd5ab658ca2193684))
- keep legacy runtime callers valid ([c23f9e2](https://github.com/0xPlayerOne/code-foundry/commit/c23f9e2980bfcb8a0b7c685f1a9ba6d26f215eba))

## [0.21.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.21.1...v0.21.2) (2026-07-28)

### Bug Fixes

- **docs:** clarify package verification ([b2bb12d](https://github.com/0xPlayerOne/code-foundry/commit/b2bb12d1674acefe5e874df280dfd083f9966e19))

## [0.21.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.21.0...v0.21.1) (2026-07-28)

### Bug Fixes

- **template:** align reusable runtime pins ([c3195e8](https://github.com/0xPlayerOne/code-foundry/commit/c3195e8a3320821c5f891ef942cf5df59ecd09bb))

## [0.21.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.20.3...v0.21.0) (2026-07-28)

### Features

- **runtime:** configure reusable workflow refs ([55f20d2](https://github.com/0xPlayerOne/code-foundry/commit/55f20d278f23ece1fed1166f1cad1b15c985ee90))

## [0.20.3](https://github.com/0xPlayerOne/code-foundry/compare/v0.20.2...v0.20.3) (2026-07-28)

### Bug Fixes

- **release-pr:** pin no-op runtime ([af662ef](https://github.com/0xPlayerOne/code-foundry/commit/af662ef7206269f03438bc3983878024629f6056))

## [0.20.2](https://github.com/0xPlayerOne/code-foundry/compare/v0.20.1...v0.20.2) (2026-07-28)

### Bug Fixes

- **release-pr:** skip empty promotions ([7c3b21b](https://github.com/0xPlayerOne/code-foundry/commit/7c3b21b19e03ac8319b1217d4e3d0d8a6f0e2317))

## [0.20.1](https://github.com/0xPlayerOne/code-foundry/compare/v0.20.0...v0.20.1) (2026-07-28)

### Bug Fixes

- **workflows:** align callers with current runtime ([11629d3](https://github.com/0xPlayerOne/code-foundry/commit/11629d32b4c41a8bfd1ff8fdaa5638c43236e889))
- **workflows:** correct release caller indentation ([2688ca9](https://github.com/0xPlayerOne/code-foundry/commit/2688ca924552c9537151e76f486f6485bd4fb0d9))

## [0.20.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.19.0...v0.20.0) (2026-07-28)

### Features

- **workflows:** use reusable promotion callers ([8429b8f](https://github.com/0xPlayerOne/code-foundry/commit/8429b8f9dee4fa0eedce2d8342332603e88e3f38))

## [0.19.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.18.0...v0.19.0) (2026-07-28)

### Features

- **workflows:** add reusable promotion runtimes ([ac113a9](https://github.com/0xPlayerOne/code-foundry/commit/ac113a902700957cbf26d4a47b4e7828b157dd13))

## [0.18.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.17.0...v0.18.0) (2026-07-28)

### Features

- **init:** infer runtime from source template ([81a545b](https://github.com/0xPlayerOne/code-foundry/commit/81a545bc6a2d89c31be51a711e477c4e4ceca7dd))

## [0.17.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.16.0...v0.17.0) (2026-07-28)

### Features

- **release:** document centralized release runtime ([3e2a3f9](https://github.com/0xPlayerOne/code-foundry/commit/3e2a3f9b5e71bf5003819aa177afd265d989bb34))

### Bug Fixes

- **release:** grant trusted publishing permission ([025f78e](https://github.com/0xPlayerOne/code-foundry/commit/025f78e851d44a60e2e4e17d3718b0b2fbe147ae))

## [0.16.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.15.0...v0.16.0) (2026-07-28)

### Features

- **release:** add reusable release workflow runtime ([19c3433](https://github.com/0xPlayerOne/code-foundry/commit/19c3433af4ae1ed796030da77f07309e2bf3e98c))

## [0.15.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.14.0...v0.15.0) (2026-07-28)

### Features

- **runtime:** unify reusable workflow pins ([bd7aece](https://github.com/0xPlayerOne/code-foundry/commit/bd7aecefac9d02be698907cba686c536c6c242d6))

## [0.14.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.13.0...v0.14.0) (2026-07-28)

### Features

- **init:** minimize consumer workflow footprint ([4427c1f](https://github.com/0xPlayerOne/code-foundry/commit/4427c1f964c3a0dc6ffe080ea3779ad2b8a1d170))

## [0.13.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.12.0...v0.13.0) (2026-07-28)

### Features

- **codeql:** document centralized CodeQL runtime ([2aa20a9](https://github.com/0xPlayerOne/code-foundry/commit/2aa20a946d0979cb12af87cb2ea2d0b50f279965))

## [0.12.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.11.0...v0.12.0) (2026-07-28)

### Features

- **codeql:** add reusable CodeQL workflow runtime ([65896bb](https://github.com/0xPlayerOne/code-foundry/commit/65896bb407ad9d792c962e86d63384849f711a16))

## [0.11.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.10.0...v0.11.0) (2026-07-28)

### Features

- **security:** document centralized security runtime ([f8427fe](https://github.com/0xPlayerOne/code-foundry/commit/f8427fe740b2753c83a400766d7dd7ac453f3c5b))

## [0.10.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.9.0...v0.10.0) (2026-07-28)

### Features

- **security:** add reusable security workflow runtime ([b21d014](https://github.com/0xPlayerOne/code-foundry/commit/b21d014e85cfcdef4181d488b1df91e3c950503b))

## [0.9.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.8.0...v0.9.0) (2026-07-28)

### Features

- **init:** configure reusable workflow repository ([95d17e9](https://github.com/0xPlayerOne/code-foundry/commit/95d17e9a4af2e2075fcdc2c357af414876655fb3))

## [0.8.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.7.0...v0.8.0) (2026-07-28)

### Features

- **test:** add reusable test workflow runtime ([5a1f4cf](https://github.com/0xPlayerOne/code-foundry/commit/5a1f4cfadb6b11f27b001ba8f6424b11de32fd64))

### Bug Fixes

- **test:** keep local workflow during runtime release ([8827659](https://github.com/0xPlayerOne/code-foundry/commit/88276590451ee6b3230ad3b1349ccd4785a686bf))

## [0.7.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.6.0...v0.7.0) (2026-07-28)

### Features

- **ci:** use reusable workflow wrapper ([77c7075](https://github.com/0xPlayerOne/code-foundry/commit/77c7075d23f48b44da276406c0000fe23c7f1dcf))

### Bug Fixes

- **ci:** declare read-only workflow permissions ([e7b7397](https://github.com/0xPlayerOne/code-foundry/commit/e7b739739979b1572760c1f81d9c7229d156c7e3))
- **ci:** name reusable checks consistently ([4a194f4](https://github.com/0xPlayerOne/code-foundry/commit/4a194f40b4f2a2660526eefac0e366402de0782d))

## [0.6.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.5.0...v0.6.0) (2026-07-28)

### Features

- **ci:** add reusable workflow runtime ([4900da5](https://github.com/0xPlayerOne/code-foundry/commit/4900da5e6141015146c4be2059bbce7da0c25f5d))

## [0.5.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.4.0...v0.5.0) (2026-07-28)

### Features

- **init:** preserve authored repository docs ([9fab688](https://github.com/0xPlayerOne/code-foundry/commit/9fab6880ad82762cf4e2eb7d813355ab22cdb905))

## [0.4.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.3.0...v0.4.0) (2026-07-28)

### Features

- **hooks:** centralize generated pre-commit runtime ([8e8111c](https://github.com/0xPlayerOne/code-foundry/commit/8e8111c1b1b95fcb356fe1b1366e369393cbf946))

## [0.3.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.2.0...v0.3.0) (2026-07-28)

### Features

- **init:** add configurable license generation ([6ea7d93](https://github.com/0xPlayerOne/code-foundry/commit/6ea7d93637620bbb2f46475eeba4789d8a3b580c))

## [0.2.0](https://github.com/0xPlayerOne/code-foundry/compare/v0.1.4...v0.2.0) (2026-07-28)

### Features

- document repository profile diagnostics ([29f132a](https://github.com/0xPlayerOne/code-foundry/commit/29f132a2b15053b06c7fe22c27324dc59151adee))

## Changelog

All notable changes to this project are documented here.
