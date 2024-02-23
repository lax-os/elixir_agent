# Modules

## NewRelic

Main entry-point/context for the NewRelic Elixir Agent.

```mermaid
classDiagram
    class NewRelic {
        +set_transaction_name(name)
        +add_attributes(custom_attributes)
        +start_transaction(category, name)
        +stop_transaction()
        +other_transaction(category, name, block)
        +ignore_transaction()
        +exclude_from_transaction()
        +get_transaction()
        +connect_to_transaction(ref)
        +disconnect_from_transaction()
        +set_span(type, attributes)
        +distributed_trace_headers(type)
        +sample_process()
        +report_custom_event(type, attributes)
        +report_dimensional_metric(type, name, value, attributes)
        +report_custom_metric(name, value)
        +increment_custom_metric(name, count)
}
```

# NewRelic.Init
Initializes [`NewRelic.Config`](#newrelicconfig) settings.



# NewRelic.Config
Maintains config state cache.
