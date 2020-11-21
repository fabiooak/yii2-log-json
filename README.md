# yii2-log-json
Extends the file logging changing the output to JSON format. It's a useful extension to integrate with FileBeat and ELK stack.

The purpose of this extension was to solve a specific problem that I had with exporting logs for use with filebeat.

After publishing this extension I found some more complete projects that solve this same problem, consider testing them if this lib doesn't meet what you need.

https://github.com/silinternational/yii2-jsonsyslog

https://github.com/urbanindo/yii2-json-log-file-target

https://github.com/index0h/yii2-log

## Usage

```php
'components' => [
    'log' => [
        'targets' => [
            [
                'class' => 'fabiooak\yii2\log\JsonFileTarget',
                'levels' => ['info', 'trace', 'error', 'warning']
            ]
        ]
    ]
]
```
