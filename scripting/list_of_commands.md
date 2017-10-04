# List of commands

#### Navigation Commands

| Command | Description |
|---------|-------------|
| [`I.goTo`](navigation.md#igoto) | Navigate to a URL |
| [`I.refreshPage`](navigation.md#irefreshpage) | Refresh a page |
| [`I.switchTab`](navigation.md#iswitchtab) | Switch Tab |

#### Mouse Commands

| Command | Description |
|---------|-------------|
| [`I.click`](mouse.md#iclick) | Click on an element |
| [`I.scrollBy`](mouse.md#iscrollby) | Scrolls the page horizontally and vertically by a given number of pixels. |
| [`I.scrollTo`](mouse.md#iscrollto) | Scrolls to a coordinate on the page |
| [`I.scrollToTop`](mouse.md#iscrolltotop) | Scroll to the top of the page |
| [`I.scrollToBottom`](mouse.md#iscrolltobottom) | Scroll to the bottom of the page |

#### Keyboard Commands

| Command | Description |
|---------|-------------|
| [`I.press`](keyboard.md#ipress) | Press a key or a string of keys |
| [`I.pressEnter`](keyboard.md#ipressenter) | Press the `Enter` key |
| [`I.pressUp`](keyboard.md#ipressup) | Press the ↑ key |
| [`I.pressDown`](keyboard.md#ipressdown) | Press the ↓ key |
| [`I.pressLeft`](keyboard.md#ipressleft) | Press the ← key |
| [`I.pressRight`](keyboard.md#ipressright) | Press the → key |

#### Form Input Commands

| Command | Description |
|---------|-------------|
| [`I.fill`](keyboard.md#ifill) | Fill a text field with a value |
| [`I.select`](keyboard.md#iselect) | Select a dropdown / checkbox / radio button |
| [`I.delect`](keyboard.md#ideselect) | Deselect a checkbox |
| [`I.upload`](keyboard.md#iupload) | Upload a file to a file field |

#### Assertion Commands

##### General assertion commands

| Command | Description |
|---------|-------------|
| [`I.see`](assertion.md#isee) | Assert that an text or element is visible |
| [`I.dontSee`](assertion.md#idontSee) | Assert that an text or element is NOT visible |

##### URL assertion commands

| Command | Description |
|---------|-------------|
| [`I.amAt`](assertion.md#iamAt) | Assert that the browser is at a specific URL |

##### Form input assertion commands

| Command | Description |
|---------|-------------|
| [`I.filled`](assertion.md#ifilled) | Assert that the form is filled with a specific value |
| [`I.selected`](assertion.md#iselected) | Assert that a dropdown option, checkbox, or radio button is selected |
| [`I.deselected`](assertion.md#ideselected) | Assert that a dropdown option, checkbox, or radio button is NOT selected |

#### Utility Commands

| Command | Description |
|---------|-------------|
| [`I.wait`](utility.md#iwait) | Wait for a given amount of time |

#### Extraction Commands

| Command | Description |
|---------|-------------|
| [`I.grabText`](extract.md#igrabtext) | Extract text from the page |

#### Sequence Commands

| Command | Description |
|---------|-------------|
| [`TEST.run`](sequence.md#testrun) | Runs another test |

