# yii2-log-json
Extends the file logging changing the output to JSON format. It's a useful extension to integrate with FileBeat and ELK stack.

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