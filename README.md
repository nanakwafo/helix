# helix
# In all environments, the following files are loaded if they exist,
# the later taking precedence over the former:
#
#  * .env                contains default values for the environment variables needed by the app
#  * .env.local          uncommitted file with local overrides
#  * .env.$APP_ENV       committed environment-specific defaults
#  * .env.$APP_ENV.local uncommitted environment-specific overrides
#
# Real environment variables win over .env files.
#
# DO NOT DEFINE PRODUCTION SECRETS IN THIS FILE NOR IN ANY OTHER COMMITTED FILES.
#
# Run "composer dump-env prod" to compile .env files for production use (requires symfony/flex >=1.2).
# https://symfony.com/doc/current/best_practices/configuration.html#infrastructure-related-configuration

SITE_URL=helix.test

###> symfony/framework-bundle ###
APP_ENV=dev
APP_SECRET=94471b6a073d4ca39130c09f8d082c5b
TRUSTED_PROXIES=helix.test,127.0.0.1
TRUSTED_HOSTS='helix.test'
###< symfony/framework-bundle ###

###> doctrine/doctrine-bundle ###
# Format described at http://docs.doctrine-project.org/projects/doctrine-dbal/en/latest/reference/configuration.html#connecting-using-a-url
# For an SQLite database, use: "sqlite:///%kernel.project_dir%/var/data.db"
# Configure your db driver and server_version in config/packages/doctrine.yaml
DATABASE_URL=pgsql://nanamensah@127.0.0.1:5432/helix
###< doctrine/doctrine-bundle ###

###> symfony/swiftmailer-bundle ###
# For Gmail as a transport, use: "gmail://username:password@localhost"
# For a generic SMTP server, use: "smtp://localhost:25?encryption=&auth_mode="
# Delivery is disabled by default via "null://localhost"
MAILER_URL=null://localhost
###< symfony/swiftmailer-bundle ###

###> google/recaptcha ###
# To use Google Recaptcha, you must register a site on Recaptcha's admin panel:
# https://www.google.com/recaptcha/admin
GOOGLE_RECAPTCHA_SITE_KEY=
GOOGLE_RECAPTCHA_SECRET=
###< google/recaptcha ###

###> snc/redis-bundle ###
# passwords that contain special characters (@, %, :, +) must be urlencoded
REDIS_URL=redis://redis
REDIS_HOST=127.0.0.1
###< snc/redis-bundle ###

ENCORE_OUTPUT_PATH='public/build/dev'

AWS_PUBLIC_BUCKET_NAME=''
AWS_PUBLIC_KEY=''
AWS_PUBLIC_SECRET=''

EMAIL_FROM='request@helixresilience.com'
EMAIL_FROM_NAME='Helix'
EMAIL_RECIPIENTS='info@helixresilience.com'

RECAPTCHA_KEY=''
