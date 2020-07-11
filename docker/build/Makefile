.RECIPEPREFIX +=

.PHONY: nothing

nothing:
	@echo Nothing to be done

# Install all dependencies defined in composer.json
install:
	composer install

update:
	composer update

# Generate dev output
all:
	vendor/bin/sculpin --project-dir=/opt --env=dev generate

