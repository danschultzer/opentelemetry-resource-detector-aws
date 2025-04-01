# OpentelemetryResourceDetectorAWS

Implements a Resource Detector for AWS.

## Installation

The package can be installed by adding `opentelemetry_resource_detector_aws` to your list of
dependencies in `mix.exs` for elixir and `rebar.config` for erlang :

```erlang
{deps, [opentelemetry_resource_detector_aws]}.
```

```elixir
def deps do
  [
    {:opentelemetry_resource_detector_aws, "~> 0.1"}
  ]
end
```

## Usage

Configure the OpenTelemetry to use the Resource Detector for AWS:

```elixir
config :opentelemetry,
    resource_detectors: [:otel_resource_aws_ecs]
```

```erlang
[
 {opentelemetry,
  [{resource_detectors, otel_resource_aws_ecs}]}
].
```

## Supported resources

- ECS (`otel_resource_aws_ecs`)

## LICENSE

(The MIT License)

Copyright (c) 2025 Dan Schultzer & the Contributors

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the 'Software'), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED 'AS IS', WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
