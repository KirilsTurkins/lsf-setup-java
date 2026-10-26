# LSF maintained setup-java security fork

Based on actions/setup-java v6.1.0 at b843ebf9b913146b38da2eaa7aeddf76074ae1ad.

Undici is overridden to 6.29.1 to fix GHSA-4qv8-2p9j-2685 and GHSA-xjj6-f33q-929c. Setup and cleanup bundles are rebuilt from the locked dependency graph. The TypeScript 6.0.3 development tarball resolves through the public npm registry with its original integrity retained.

Build: Node 24.19.0, npm ci --ignore-scripts, npm run build. Validation: all 45 upstream suites, 1,566 tests passed and two upstream skips. OSV reports no findings in 44 production packages. LSF-SECURITY.json records source, tool and bundle identities.

The upstream MIT license and source history are retained. Review and rebuild when refreshing upstream source or the dependency graph.
