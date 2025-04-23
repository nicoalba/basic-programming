# Therapy Bot SDK Doc

## Programming for Writers — 4/19/2020

### Constants

| Name                   | Description                                                        | Type             |
| ---------------------- | ------------------------------------------------------------------ | ---------------- |
| `exclamationResponses` | Responses for when the user's line ends with an exclamation point. | Array of strings |
| `genericResponses`     | Responses to use when there are no better options.                 | Array of strings |
| `povSwitches`          | Mapping between first person and second person words.              | Object           |
| `questionResponses`    | Responses for when the user's line ends with a question mark.      | Array of strings |
| `questionStarts`       | First few words of a question.                                     | Array of strings |

### Functions

| Name                          | Description                                     | Parameters                                                             | Returns                                                           |
| ----------------------------- | ----------------------------------------------- | ---------------------------------------------------------------------- | ----------------------------------------------------------------- |
| `createQuestion(patientLine)` | Returns a question based on the patient's line. | `-patientLine`<br> Type: string <br> The patient's text to respond to. | Type: string <br> A question based on the patient's line.         |
| `lastChar(myString)`          | Returns the last character in a string.         | `-myString`<br> Type: string <br> String to return last character for. | Type: string <br> Last character of the string.                   |
| `randomElement(myArray)`      | Returns a random element of an array.           | `-myArray`<br> Type: array <br> Array with one or more elements.       | Type: whatever is in the array <br>Random element from the array. |

### Enumerations

| Name          | Description                                                                                                      | Value |
| ------------- | ---------------------------------------------------------------------------------------------------------------- | ----- |
| `Generic`     | Generic answer that does not make use ofthe patient response.                                                    | 0     |
| `Question`    | Answer to a question.                                                                                            | 1     |
| `Exclamation` | Answer to a patient response that ends with an exclamation point.                                                | 2     |
| `PointOfView` | Answer that makes use of the patient response by switching the point of view from first person to second person. | 3     |
