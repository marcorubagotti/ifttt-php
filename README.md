# ifttt-php
Ifttt php class for [Maker Webhooks](https://ifttt.com/maker_webhooks)

```
<?php

require 'ifttt-php.class.php';

$maker = new Maker('event_name', 'ifttt_apikey');

// set values to send, optional
$values = array(
  'value1' => 'my first value',
  'value2' => 'my second value',
  'value3' => 'my third value'
);
$maker->set_values($values);

// trigger the ifttt event
if($maker->trigger()){
  echo 'event triggered!';
}

...
```
