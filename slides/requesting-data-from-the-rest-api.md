##  Requesting data from the REST API

<pre><code class="hljs">
  public function build() {
    $options = [
      'query' => [
        'type' => 'changenotice',
        'limit' => 5,
        'status' => 1,
        'sort' => 'created',
        'direction' => 'DESC',
      ],
    ];
    $result = $this->httpClient->get('https://www.drupal.org/api-d7/node.json', $options);
    $change_records = json_decode($result->getBody())->list;
    // ...
  }
</code></pre>
