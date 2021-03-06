## test

Run all the tests

```sh
pytest
```

## test-debug

Run all the tests with `debug` logger.

```sh
pytest --log-cli-level debug
```

## test-coverage

```sh
py.test --cov-report term-missing --cov=bbox tests/ 
```

## generate-docs

```sh
make -C docsrc html
```

## publish-docs

Run task `generate-docs` before this

```sh
rm -rf docs
cp -a docsrc/build/html docs
```

## build

```sh
poetry build
```

## publish

Run task `build` before this

```sh
echo "publishing"
poetry publish
```