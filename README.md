# vitest-polly

Recording functionality for Vitest with Polly

## Requirements

Requires one of:

- **vitest** >= 4.1.0
- **vite-plus** >= 0.1.14

## Installation

```sh
npm install vitest-polly
```

## Usage

```ts
import { test, expect } from "vitest"
import { useRecording } from "vitest-polly"

useRecording({
  recordingName: "optional-name",
  recordingPath: "optional-path",
})

test("fetches a user", async () => {
  const response = await fetch("https://jsonplaceholder.typicode.com/users/1")
  expect(response.status).toBe(200)
})
```

## Credits

- A solution by [ekrata-main](https://github.com/ekrata-main) and [damonbauer](https://github.com/damonbauer) from [pollyjs#499](https://github.com/Netflix/pollyjs/issues/499#issuecomment-2254483748).
