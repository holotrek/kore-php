# Kore (Kaiser-Core) PHP library

NOTE: This is currently a placeholder repository for a **Work-in-Progress**

## Synopsis

Core cross-cutting Providers and other common functions for PHP projects.

## Download

This is a library provided for use within a project and is not an independent application. The best way to include the library in your project is to use Composer:

[Composer download command TBD]

## Features

### Providers

Kore-PHP contains contracts for cross-cutting concerns that are commonly used by every application. Specific implementations of these contracts will be included in separate projects so that you can choose which implementation fits your project best. Implementations are explained in sub-bullet points beneath each provider.

Current list of providers:
* **Authentication**: Provides a common set of methods to use for authentication.
  * Forms [TBD]
  * oAuth [TBD]
* **Caching**: Provides a basic common set of methods for putting things in a cache and retrieving them by key.
  * Doctrine Cache [TBD]
* **Containers**: This is a wrapper for which IoC container you use, so that the Kore can use it to resolve objects. Mainly only used if you want to use the Domain Event Dispatching functionality.
  * PHP-DI [TBD]
* **Email**: The Kore has a basic email provider that will use native PHP mail(). It provides a contract however, for the common emailing methods that can be used in a specific implementation.
  * SendGrid [TBD]
* **Logging**: Methods for logging different severity messages to a logging provider. Can be injected into the Messages provider to have any messages be automatically logged.
  * Monolog [TBD]
* **Messages**: Methods for collecting messages from any layer of the application (Controller/Service/Domain) and providing the ability to link them to a certain property and/or GUID. This provider works out of the box with Kore using the base implementation, so a separate library below is not strictly required.
  * [TBD]
* **PDF Manipulation**: Description TBD
  * TCPDF [TBD]
* **Serialization**: Methods to serialize/deserialize objects to and from JSON. The default provider will use the native json_encode() and json_decode() functions.

More features TBD...

## Contributing

TBD (will provide info once project is complete and uploaded)

## License

See [LICENSE](LICENSE)
