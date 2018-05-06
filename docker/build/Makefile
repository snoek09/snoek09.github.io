.RECIPEPREFIX +=

.PHONY: nothing

nothing:
    @echo Nothing to be done

# Install all dependencies defined in composer.json
install:
    composer install

# Process all source files
all:
    vendor/bin/sculpin --project-dir=/opt --env=prod generate

