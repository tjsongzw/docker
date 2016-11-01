RELEASE = base

all: test

build:
	docker build -t data-py3:$(RELEASE) .

test:
	docker run data-py3:$(RELEASE) python -c 'import pandas; print(pandas.__version__)'
