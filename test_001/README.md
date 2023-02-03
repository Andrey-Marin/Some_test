Сhecking file storage location to run container script.

#### Preparation

**Step 1:** create docker images.

    docker build -t test:v001 .

**Step 2:** run docker container.

    docker run --rm test:v001

#### Result

    Hello, Ann
    Hello, Andrew
    Hello, Kirill

But, if we change the [names.txt](./names.txt) file, we will also get the previos result.
Because docker saved the file inside itself.

To fix this, you need to explicitly specify the file when starting the container.

    docker run --rm -v $(pwd)/names.txt:/app/names.txt test:v001

#### New result

    Hello, Ann
    Hello, Andrew
    Hello, Kirill
    Hello, Anton
