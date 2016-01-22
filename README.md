# Reading Time
Estimated reading time plugin for Fansoro

## Installation
See [this instruction](http://fansoro.org/documentation/plugins/plugins-installation)

## Usage

Simple usage  

```smarty
{readingTime($post.content)}
```

Localization  

```smarty
{readingTime($post.content, [
    'minute'  => 'Minute',
    'minutes' => 'Minutes',
    'second'  => 'Second',
    'seconds' => 'Seconds'])}
```

Set custom format of the result   

```smarty
{readingTime($post.content, [
    'minute'  => 'Minute',
    'minutes' => 'Minutes',
    'second'  => 'Second',
    'seconds' => 'Seconds',
    'format'  => '{minutes_count} {minutes_label} – {seconds_count} {seconds_label}'])}
```

Enable alternative format that hides the minute label.

```smarty
{readingTime($post.content, [
    'format' => '{minutes_count} {minutes_label}, {seconds_count} {seconds_label}',
    'format.alt' => '{seconds_count} {seconds_label}',
    'format.alt.enable' => true])}
```

## License
See [LICENSE](https://github.com/fansoro/fansoro-plugin-reading-time/blob/master/LICENSE)
