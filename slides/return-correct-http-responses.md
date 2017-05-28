##  Return correct HTTP responses

  <ul>
    <li><code class="inline-code">200 OK</code> - Successful GET or PATCH</li>
    <li><code class="inline-code">201 Created</code> - Successful POST</li>
    <li><code class="inline-code">204 No Content</code> - Successful DELETE</li>
    <li><code class="inline-code">400 Bad Request</code> - Invalid data received</li>
    <li><code class="inline-code">401 Unauthorized</code> - Not authenticated</li>
    <li><code class="inline-code">403 Forbidden</code> - Successfully authenticated, no access</li>
    <li><code class="inline-code">404 Not Found</code> - Resource does not exist</li>
    <li><code class="inline-code">405 Method Not Allowed</code> - Successfully authenticated, wrong HTTP method</li>
    <li><code class="inline-code">410 Gone</code> - API version is deprecated</li>
    <li><code class="inline-code">422 Unprocessable Entity</code> - Validation error</li>
    <li><code class="inline-code">429 Too Many Requests</code> - Exceeded rate limiting</li>
  </ul>
