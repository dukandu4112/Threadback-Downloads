# Third-party components

Threadback's application source is private. The third-party source download contains upstream dependency sources, not Threadback source.

| Component | Version | Notices and source |
|---|---|---|
| OpenJFX controls, graphics, base and native libraries | 17.0.16 | Upstream GPL v2 with Classpath Exception and component-specific notices; full upstream archive in ThirdPartySources |
| Xerial SQLite JDBC and bundled native SQLite libraries | 3.47.1.0 | Apache 2.0, legacy driver and component-specific notices; full upstream archive in ThirdPartySources |
| Eclipse Temurin Java runtime | 17.0.20+8 | Runtime notices in runtime/legal; full supplier source archive in ThirdPartySources |

Read the actual upstream notices in `third-party-notices` and `runtime/legal` for the applicable terms and third-party attributions. `COMPONENTS.json` records the resolved binary dependency files, source locations, and SHA-256 hashes. The separate **ThirdPartySources.zip** asset is available alongside the Windows ZIP, without charge.

The application combines these unmodified components with Threadback's application code. The dependency source bundles include their upstream build files. No claim is made that Threadback's private application source is covered by an open-source license.
