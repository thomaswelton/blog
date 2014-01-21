# Using less source maps with Symfony

```php
class LessFilter extends AsseticLessFilter
{
    public function filterLoad(AssetInterface $asset)
    {
        $sourcemapRoot = realpath(dirname($asset->getSourceRoot() . '/' . $asset->getSourcePath()));

        $this->addTreeOption('sourceMap', true);
        $this->addTreeOption('sourceMapBasepath', $sourcemapRoot);

        parent::filterLoad($asset);
    }
}
```

```yml
assetic:
    filters:
        less:
            class: "Moo\\M4BBundle\\Assetic\\LessFilter"
```
