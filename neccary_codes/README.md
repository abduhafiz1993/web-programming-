# fetch

Response properties:

response.status – HTTP code of the response,
response.ok – true if the status is 200-299.
response.headers – Map-like object with HTTP headers.
Methods to get response body:

response.text() – return the response as text,
response.json() – parse the response as JSON object,
response.formData() – return the response as FormData object (multipart/form-data encoding, see the next chapter),
response.blob() – return the response as Blob (binary data with type),
response.arrayBuffer() – return the response as ArrayBuffer (low-level binary data),
Fetch options so far:

method – HTTP-method,
headers – an object with request headers (not any header is allowed),
body – the data to send (request body) as string, FormData, BufferSource, Blob or UrlSearchParams object.
In the next chapters we’ll see more options and use cases of fetch