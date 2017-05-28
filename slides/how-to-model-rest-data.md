##  How to model REST data

<ul>
  <li>Create custom entity representing REST data</li>
  <li>Inject the 'serializer' service</li>
  <li>Deserialize the REST data into an entity</li>
</ul>

<pre><code class="hljs">
 $data = $this->httpClient->get('https://www.drupal.org/api-d7/node/2692565.json');
 $serializer = \Drupal::service('serializer');
 $entity = $serializer->deserialize($data, 'Drupal\change_records\Entity\ChangeRecord', 'json');

</code></pre>
