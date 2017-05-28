##  Returning a JSON response

<pre><code class="hljs">
class RestApiController extends ControllerBase {

  use Symfony\Component\HttpFoundation\JsonResponse;

  public function getStats($date_range) {
    $data = [
      'unique_visitors' => 100,
      'page_views' => 3440,
      'date_range' => ['2016-03-15T08:14:45Z', '2016-04-15T08:14:45Z'],
    ];
    return new JsonResponse($data);
  }

}
</code></pre>
