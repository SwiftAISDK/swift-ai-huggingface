<!-- Generated distribution; edit the canonical repository. -->
# swift-ai-huggingface 1.0.0

Independent Swift-native port of Vercel AI SDK. Source and upstream dispositions are in PROVENANCE.json and Porting/.

## Distribution manifest

Add this package to your SwiftPM dependencies:

```swift
.package(url: "https://github.com/SwiftAISDK/swift-ai-huggingface.git", from: "1.0.0")
```

Products: `SwiftAIHuggingFace`.
Contribute and report issues in the canonical SwiftAISDK repository.

## Authored usage guide

# SwiftAIHuggingFace

Swift-native port of `@ai-sdk/huggingface`. Maintained in the canonical SwiftAISDK repository and exported as an independent Swift package.

```swift
import SwiftAIHuggingFace

let provider = try HuggingFaceProvider(configuration: .init(apiKey: "..."))
```

Settings accept a custom base URL, headers, query parameters and an injected
`AITransport`. Models use the common SwiftAIProvider protocols. Existing upstream
baselines, capabilities and documented gaps remain unchanged.

Run the standalone suite from the canonical checkout:

```sh
swift test --package-path Packages/swift-ai-huggingface
```

The canonical repository owns all edits. Distribution manifests and repositories
are generated from the catalog; see `Porting/map.json` and the canonical provider guide.

See [provider usage and capabilities](https://github.com/SwiftAISDK/SwiftAISDK/blob/main/docs-site/scripts/provider-guides/huggingface.md) for authentication, options and supported surfaces.
