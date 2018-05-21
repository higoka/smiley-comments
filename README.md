# Smiley Comments
Addon to use for BrainCMS that adds smileys support to the comments.

Example: https://picr.ws/i/rsn

### Setup
Download the ZIP file and extract it. Replace all the files with the files from BrainCMS.
Next, add this code at the bottom of the file `system/brain-config.php`. (Above ?>)

```php
/**
 * Smiley Addon
 */
$config['smileys'] = [
    /**
     * Enable / disable the smileys
     */
    'enabled' => true,

    /**
     * Directory where the smileys are stored.
     */
    'directory' => '/templates/brain/style/images/smileys',

    /**
     * Add your own replacements
     */
    'replacements' => [
        ':)'     => 'smiling.svg',
        ':('     => 'sad.svg',
        ';)'     => 'wink.svg',
        ':P'     => 'tongue-out-1.svg',
        ':D'     => 'happy-1.svg',
        ':\'('   => 'unhappy.svg',
        '&gt;:(' => 'angry.svg',
        ':*'     => 'kissing.svg',
    ],
];
```

If done correctly, you now have setup smiley in the comments.

### Contribute
Contribution, bug fixes etc are [always welcome](https://github.com/higoka/smiley-comments/issues/new).

### Credits
- [Higoka](https://github.com/higoka)
- [All Contributors](https://github.com/higoka/smiley-comments/contributors)

### License
The MIT License (MIT).
Please see [License File](https://github.com/higoka/smiley-comments/blob/master/LICENSE) for more information.
