#OnlineMarketingApiToolkit: SemrushClient

Der SEMrush-Client beinhaltet alle Endpoints der API unter: http://de.semrush.com/api.html

Beispiel:

```php
use Zedwoo\OnlineMarketingApiToolkit\Moz\SemrushClient
$client = SemrushClient::factory(array( 'api_key' => 'YOUR_API_KEY'
								));
$command = $client->getCommand('domain_organic', array(
												   'domain' => 'chefkoch.de',
												   'display_limit' => 100
											  ));
$result = $command->execute(); // returns an array with the result
```

Weitere Infos bietet die entsprechende JSON-Datei:
[ServiceDescriptionSemrush.json](https://github.com/zedwoo/online-marketing-api-toolkit/blob/master/src/Zedwoo/OnlineMarketingApiToolkit/Semrush/Resources/ServiceDescriptionSemrush.json)
