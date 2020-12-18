# subtitles

Parse or generate various subtitle formats in Swift.

## Usage
```swift
let genericSubtitleFile = GenericSubtitleFile(subtitles: [
    .init(text: "Everything was dark...", start: 0, end: 1.95),
    .init(text: "and then...", start: 1.95, end: 3.0),
    .init(text: "LIGHT", start: 3.0, end: 3.7)
])

let file = try SubtitleFile(file: genericSubtitleFile, kind: .srt)
let string = file.asString()
```
