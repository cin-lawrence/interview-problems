# Problem 2
To provide reasoning for a question in an AI chat application, the internal AI pipeline requires chunks of “Evidence” for processing. Evidence could be either a paragraph or an image, they are given from a separate service named Extractor.
Extractor could handle a wide range of file extensions given to it.
- The service receives a file via an HTTP POST request.
- If the file format is supported
  - The service breaks the file down into Pages.
  - The service processes Pages into multiple Evidence.
- If the file format is unknown
  - The service should try to guess the file extension to see if processing is feasible.
  - If the service is unable to process the file, it should return an error code.

The evidence extracted could be passed into another function call, persisted into database or file storage, or serialized.

In this problem:
- There are 5 default supported extensions: DOCX, PDF, HTML, PPTX (PPT), TIFF (TIF).
- Future extensions might be added: XLSX, CSV.
- Different ways of handling a file extension might be added.
- There are 2 potential Evidence types: Paragraph and Image.
- Additional Evidence types might be added in the future.

Implement the following requirements using the programming language of your choice, preferably Python if you can.


## Implementation scope
- The detailed logic of handling each extension should be ignored. Use pseudo-code only.
- The implementation should demonstrate a good way of handling exceptions.


## Implementation requirements
The implementation should satisfy the following criteria:
- Leveraging OOP as much as it could.
- Convenience for both maintaining and extending the code base.
- Providing the simplest facade for another developer.
  - When they use the extraction code internally without an API handler.
  - When they reuse the code with new extensions.
  - When they reuse the code with a different strategy for an existing extension.
- Recoverability (handling exceptions properly).
- Test-driven.


## Bonus
- Typing
- Modulizing
- Asynchronous programming
