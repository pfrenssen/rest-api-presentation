##  Returning the data

<pre><code class="hljs">
  public function build() {
    // ...
    $items = [];
    foreach ($change_records as $change_record) {
      $items[] = [
        '#type' => 'link',
        '#title' => $change_record->title,
        '#url' => Url::fromUri($change_record->url),
      ];
    }
    return [
      '#theme' => 'item_list',
      '#items' => $items,
      '#list_type' => 'ol',
    ];
  }
</code></pre>
