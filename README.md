# vitest-polly

Recording functionality for Vitest with Polly

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
