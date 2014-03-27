# New Ruby 2.1 awesomness: pro object allocation tracing

Sam Rawlins, @srawlins

ObjectSpace.trace_object_allocation

Useful but limited.

Aggregated stats gem? srawlins on github? `require "allocation_stats"`

Rack middleware looks really cool too

Ruby array addition creates a new array and then appends; Array.concat does not.

String#freeze - string literals when frozen will always refer to the same object. Doesn't allocate objects the second time through.

google this - github blog post hey judy
