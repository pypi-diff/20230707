# Comparing `tmp/bus_station-6.1.1.tar.gz` & `tmp/bus_station-6.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bus_station-6.1.1.tar", max compression
+gzip compressed data, was "bus_station-6.1.2.tar", max compression
```

## Comparing `bus_station-6.1.1.tar` & `bus_station-6.1.2.tar`

### file list

```diff
@@ -1,161 +1,162 @@
--rw-r--r--   0        0        0       48 2023-07-04 22:41:45.243617 bus_station-6.1.1/README.md
--rw-r--r--   0        0        0      985 2023-07-04 22:43:18.357100 bus_station-6.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/__init__.py
--rw-r--r--   0        0        0      143 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/bus_stop.py
--rw-r--r--   0        0        0      692 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/environment.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/address/__init__.py
--rw-r--r--   0        0        0      199 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/address/address_not_found_for_bus_stop.py
--rw-r--r--   0        0        0      407 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
--rw-r--r--   0        0        0      673 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
--rw-r--r--   0        0        0     3526 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/bus_stop_registry.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/supervisor/__init__.py
--rw-r--r--   0        0        0     1180 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py
--rw-r--r--   0        0        0      255 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/registration/supervisor/bus_stop_registration_supervisor.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/resolvers/__init__.py
--rw-r--r--   0        0        0      289 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/resolvers/bus_stop_resolver.py
--rw-r--r--   0        0        0      614 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py
--rw-r--r--   0        0        0      811 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py
--rw-r--r--   0        0        0     1146 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/command_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/command_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.243617 bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1352 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
--rw-r--r--   0        0        0      889 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
--rw-r--r--   0        0        0     1237 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
--rw-r--r--   0        0        0      258 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/command_bus.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2315 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
--rw-r--r--   0        0        0     2188 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
--rw-r--r--   0        0        0     1128 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1326 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
--rw-r--r--   0        0        0     2747 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
--rw-r--r--   0        0        0     1856 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
--rw-r--r--   0        0        0     1266 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
--rw-r--r--   0        0        0      253 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/command.py
--rw-r--r--   0        0        0      292 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/command_execution_failed.py
--rw-r--r--   0        0        0      457 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/command_handler.py
--rw-r--r--   0        0        0      227 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/command_handler_not_found.py
--rw-r--r--   0        0        0     1510 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/command_handler_registry.py
--rw-r--r--   0        0        0      233 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/handler_not_found_for_command.py
--rw-r--r--   0        0        0      725 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/json_rpc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      607 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/middleware/command_middleware.py
--rw-r--r--   0        0        0     1078 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1070 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
--rw-r--r--   0        0        0     1039 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
--rw-r--r--   0        0        0      890 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
--rw-r--r--   0        0        0      712 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/command_terminal/rpyc_command_server.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
--rw-r--r--   0        0        0     1247 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
--rw-r--r--   0        0        0     1212 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
--rw-r--r--   0        0        0      984 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
--rw-r--r--   0        0        0      246 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/event_bus.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0      872 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     3196 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
--rw-r--r--   0        0        0     1625 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
--rw-r--r--   0        0        0      249 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/event.py
--rw-r--r--   0        0        0      446 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/event_consumer.py
--rw-r--r--   0        0        0      221 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/event_consumer_not_found.py
--rw-r--r--   0        0        0     1439 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/event_consumer_registry.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/middleware/__init__.py
--rw-r--r--   0        0        0      590 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/middleware/event_middleware.py
--rw-r--r--   0        0        0     1049 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1038 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
--rw-r--r--   0        0        0     1012 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
--rw-r--r--   0        0        0      864 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/__init__.py
--rw-r--r--   0        0        0     1440 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/memory_queue_passenger_worker.py
--rw-r--r--   0        0        0     2319 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/passenger.py
--rw-r--r--   0        0        0     2042 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/passenger_kombu_consumer.py
--rw-r--r--   0        0        0     2294 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/passenger_mapper.py
--rw-r--r--   0        0        0       76 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/passenger_middleware.py
--rw-r--r--   0        0        0      637 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/passenger_registry.py
--rw-r--r--   0        0        0      641 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/passenger_resolvers.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/reception/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/reception/passenger_middleware_receiver.py
--rw-r--r--   0        0        0      792 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/reception/passenger_receiver.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/serialization/__init__.py
--rw-r--r--   0        0        0      347 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/serialization/passenger_deserialization_error.py
--rw-r--r--   0        0        0      321 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/serialization/passenger_deserializer.py
--rw-r--r--   0        0        0     1016 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/serialization/passenger_json_deserializer.py
--rw-r--r--   0        0        0      822 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/serialization/passenger_json_serializer.py
--rw-r--r--   0        0        0      241 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/passengers/serialization/passenger_serializer.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus/__init__.py
--rw-r--r--   0        0        0      323 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus/query_bus.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
--rw-r--r--   0        0        0     2671 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
--rw-r--r--   0        0        0     2580 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
--rw-r--r--   0        0        0     1127 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus_engine/__init__.py
--rw-r--r--   0        0        0     1242 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
--rw-r--r--   0        0        0     1218 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
--rw-r--r--   0        0        0      219 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/handler_not_found_for_query.py
--rw-r--r--   0        0        0     1483 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/json_rpc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/middleware/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/middleware/implementations/__init__.py
--rw-r--r--   0        0        0     1261 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
--rw-r--r--   0        0        0     1178 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
--rw-r--r--   0        0        0     1227 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
--rw-r--r--   0        0        0      726 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/middleware/query_middleware.py
--rw-r--r--   0        0        0     1286 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
--rw-r--r--   0        0        0      249 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/query.py
--rw-r--r--   0        0        0      273 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/query_execution_failed.py
--rw-r--r--   0        0        0      520 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/query_handler.py
--rw-r--r--   0        0        0      215 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/query_handler_not_found.py
--rw-r--r--   0        0        0     1480 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/query_handler_registry.py
--rw-r--r--   0        0        0      138 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/query_response.py
--rw-r--r--   0        0        0     1442 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/rpyc_query_server.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/serialization/__init__.py
--rw-r--r--   0        0        0      282 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/serialization/query_response_deserializer.py
--rw-r--r--   0        0        0      465 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
--rw-r--r--   0        0        0      390 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
--rw-r--r--   0        0        0      267 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/query_terminal/serialization/query_response_serializer.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/broker_connection/__init__.py
--rw-r--r--   0        0        0      352 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
--rw-r--r--   0        0        0      176 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
--rw-r--r--   0        0        0     1249 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
--rw-r--r--   0        0        0      695 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/bus.py
--rw-r--r--   0        0        0      438 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/context.py
--rw-r--r--   0        0        0      118 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/dataclass_type.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/engine/__init__.py
--rw-r--r--   0        0        0      181 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/engine/engine.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/engine/runner/__init__.py
--rw-r--r--   0        0        0      436 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/engine/runner/engine_runner.py
--rw-r--r--   0        0        0      805 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
--rw-r--r--   0        0        0      241 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/factories/__init__.py
--rw-r--r--   0        0        0      381 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
--rw-r--r--   0        0        0      545 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/factories/memory_queue_factory.py
--rw-r--r--   0        0        0      305 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/fqn.py
--rw-r--r--   0        0        0     2493 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/json_rpc_server.py
--rw-r--r--   0        0        0      956 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/kafka_topic_creator.py
--rw-r--r--   0        0        0     2037 2023-07-04 22:41:45.247617 bus_station-6.1.1/src/bus_station/shared_terminal/rpyc_server.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/__init__.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/__init__.py
--rw-r--r--   0        0        0      185 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/command_tracking.py
--rw-r--r--   0        0        0      183 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/event_tracking.py
--rw-r--r--   0        0        0      950 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
--rw-r--r--   0        0        0      347 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/passenger_tracking.py
--rw-r--r--   0        0        0      744 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
--rw-r--r--   0        0        0      297 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
--rw-r--r--   0        0        0      281 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/models/query_tracking.py
--rw-r--r--   0        0        0        0 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/trackers/__init__.py
--rw-r--r--   0        0        0     1400 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
--rw-r--r--   0        0        0     2483 2023-07-04 22:41:45.251617 bus_station-6.1.1/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
--rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 bus_station-6.1.1/PKG-INFO
+-rw-r--r--   0        0        0       48 2023-07-07 08:30:00.373248 bus_station-6.1.2/README.md
+-rw-r--r--   0        0        0      985 2023-07-07 08:31:33.988417 bus_station-6.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/__init__.py
+-rw-r--r--   0        0        0      143 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/bus_stop.py
+-rw-r--r--   0        0        0      185 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/bus_stop_not_found.py
+-rw-r--r--   0        0        0      692 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/environment.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/__init__.py
+-rw-r--r--   0        0        0      199 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/address_not_found_for_bus_stop.py
+-rw-r--r--   0        0        0      407 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/bus_stop_address_registry.py
+-rw-r--r--   0        0        0      673 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py
+-rw-r--r--   0        0        0     3774 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/bus_stop_registry.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/__init__.py
+-rw-r--r--   0        0        0     1180 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py
+-rw-r--r--   0        0        0      255 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/bus_stop_registration_supervisor.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/__init__.py
+-rw-r--r--   0        0        0      250 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/bus_stop_resolver.py
+-rw-r--r--   0        0        0      587 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py
+-rw-r--r--   0        0        0      772 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py
+-rw-r--r--   0        0        0     1107 2023-07-07 08:30:00.373248 bus_station-6.1.2/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1352 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py
+-rw-r--r--   0        0        0      889 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py
+-rw-r--r--   0        0        0     1237 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py
+-rw-r--r--   0        0        0      258 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2315 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py
+-rw-r--r--   0        0        0     2188 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py
+-rw-r--r--   0        0        0     1128 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1326 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py
+-rw-r--r--   0        0        0     2747 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py
+-rw-r--r--   0        0        0     1856 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py
+-rw-r--r--   0        0        0     1266 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py
+-rw-r--r--   0        0        0      253 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command.py
+-rw-r--r--   0        0        0      292 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_execution_failed.py
+-rw-r--r--   0        0        0      457 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_handler.py
+-rw-r--r--   0        0        0      227 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_handler_not_found.py
+-rw-r--r--   0        0        0     1795 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/command_handler_registry.py
+-rw-r--r--   0        0        0      233 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/handler_not_found_for_command.py
+-rw-r--r--   0        0        0      725 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/json_rpc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      607 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware.py
+-rw-r--r--   0        0        0     1078 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1070 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py
+-rw-r--r--   0        0        0     1039 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py
+-rw-r--r--   0        0        0      890 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py
+-rw-r--r--   0        0        0      712 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/command_terminal/rpyc_command_server.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     1247 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py
+-rw-r--r--   0        0        0     1212 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py
+-rw-r--r--   0        0        0      984 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py
+-rw-r--r--   0        0        0      246 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0      872 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     3196 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py
+-rw-r--r--   0        0        0     1625 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py
+-rw-r--r--   0        0        0      249 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event.py
+-rw-r--r--   0        0        0      446 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event_consumer.py
+-rw-r--r--   0        0        0      221 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event_consumer_not_found.py
+-rw-r--r--   0        0        0     1439 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/event_consumer_registry.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware.py
+-rw-r--r--   0        0        0     1049 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1038 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py
+-rw-r--r--   0        0        0     1012 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py
+-rw-r--r--   0        0        0      864 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/__init__.py
+-rw-r--r--   0        0        0     1440 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/memory_queue_passenger_worker.py
+-rw-r--r--   0        0        0     2319 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger.py
+-rw-r--r--   0        0        0     2042 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_kombu_consumer.py
+-rw-r--r--   0        0        0     2294 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_mapper.py
+-rw-r--r--   0        0        0       76 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_middleware.py
+-rw-r--r--   0        0        0      637 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_registry.py
+-rw-r--r--   0        0        0      641 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/passenger_resolvers.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/reception/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/reception/passenger_middleware_receiver.py
+-rw-r--r--   0        0        0      792 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/reception/passenger_receiver.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/__init__.py
+-rw-r--r--   0        0        0      347 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_deserialization_error.py
+-rw-r--r--   0        0        0      321 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_deserializer.py
+-rw-r--r--   0        0        0     1016 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_deserializer.py
+-rw-r--r--   0        0        0      822 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_serializer.py
+-rw-r--r--   0        0        0      241 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/__init__.py
+-rw-r--r--   0        0        0      323 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/__init__.py
+-rw-r--r--   0        0        0     2671 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py
+-rw-r--r--   0        0        0     2580 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py
+-rw-r--r--   0        0        0     1127 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/__init__.py
+-rw-r--r--   0        0        0     1242 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py
+-rw-r--r--   0        0        0     1218 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py
+-rw-r--r--   0        0        0      219 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/handler_not_found_for_query.py
+-rw-r--r--   0        0        0     1483 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/json_rpc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/__init__.py
+-rw-r--r--   0        0        0     1261 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py
+-rw-r--r--   0        0        0     1178 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py
+-rw-r--r--   0        0        0     1227 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py
+-rw-r--r--   0        0        0      726 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware.py
+-rw-r--r--   0        0        0     1286 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware_receiver.py
+-rw-r--r--   0        0        0      249 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query.py
+-rw-r--r--   0        0        0      273 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_execution_failed.py
+-rw-r--r--   0        0        0      520 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_handler.py
+-rw-r--r--   0        0        0      215 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_handler_not_found.py
+-rw-r--r--   0        0        0     1747 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_handler_registry.py
+-rw-r--r--   0        0        0      138 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/query_response.py
+-rw-r--r--   0        0        0     1442 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/rpyc_query_server.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/__init__.py
+-rw-r--r--   0        0        0      282 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_deserializer.py
+-rw-r--r--   0        0        0      465 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_json_deserializer.py
+-rw-r--r--   0        0        0      390 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_json_serializer.py
+-rw-r--r--   0        0        0      267 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/query_terminal/serialization/query_response_serializer.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/__init__.py
+-rw-r--r--   0        0        0      352 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/broker_connection_type.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/__init__.py
+-rw-r--r--   0        0        0      176 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/connection_parameters.py
+-rw-r--r--   0        0        0     1249 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py
+-rw-r--r--   0        0        0      695 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/bus.py
+-rw-r--r--   0        0        0      438 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/context.py
+-rw-r--r--   0        0        0      118 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/dataclass_type.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/__init__.py
+-rw-r--r--   0        0        0      181 2023-07-07 08:30:00.377248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/engine.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/__init__.py
+-rw-r--r--   0        0        0      436 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/engine_runner.py
+-rw-r--r--   0        0        0      805 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py
+-rw-r--r--   0        0        0      241 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/self_process_engine_runner.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/factories/__init__.py
+-rw-r--r--   0        0        0      381 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/factories/kombu_connection_factory.py
+-rw-r--r--   0        0        0      545 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/factories/memory_queue_factory.py
+-rw-r--r--   0        0        0      305 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/fqn.py
+-rw-r--r--   0        0        0     2493 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/json_rpc_server.py
+-rw-r--r--   0        0        0      956 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/kafka_topic_creator.py
+-rw-r--r--   0        0        0     2037 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/shared_terminal/rpyc_server.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/__init__.py
+-rw-r--r--   0        0        0      185 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/command_tracking.py
+-rw-r--r--   0        0        0      183 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/event_tracking.py
+-rw-r--r--   0        0        0      950 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py
+-rw-r--r--   0        0        0      347 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking.py
+-rw-r--r--   0        0        0      744 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py
+-rw-r--r--   0        0        0      297 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking_serializer.py
+-rw-r--r--   0        0        0      281 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/models/query_tracking.py
+-rw-r--r--   0        0        0        0 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/__init__.py
+-rw-r--r--   0        0        0     1400 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py
+-rw-r--r--   0        0        0     2483 2023-07-07 08:30:00.381248 bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/passenger_tracker.py
+-rw-r--r--   0        0        0      746 1970-01-01 00:00:00.000000 bus_station-6.1.2/PKG-INFO
```

### Comparing `bus_station-6.1.1/pyproject.toml` & `bus_station-6.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bus-station"
-version = "6.1.1"
+version = "6.1.2"
 description = "A python bus station"
 readme = "README.md"
 authors = ["DeejayRevok <seryi_one@hotmail.com>"]
 
 [tool.poetry.dependencies]
 python = "~=3.10.0"
 kombu = "5.2.2"
@@ -41,15 +41,15 @@
 [tool.isort]
 profile = "black"
 py_version=310
 line_length = 120
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "6.1.1"
+version = "6.1.2"
 tag_format = "$version"
 version_files = [
   "pyproject.toml:version"
 ]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `bus_station-6.1.1/src/bus_station/bus_stop/environment.py` & `bus_station-6.1.2/src/bus_station/bus_stop/environment.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py` & `bus_station-6.1.2/src/bus_station/bus_stop/registration/address/redis_bus_stop_address_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/bus_stop/registration/bus_stop_registry.py` & `bus_station-6.1.2/src/bus_station/bus_stop/registration/bus_stop_registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+# pyre-ignore-all-errors[7]
 from typing import Callable, Dict, Generic, List, Optional, Set, TypeVar
 
 from bus_station.bus_stop.bus_stop import BusStop
+from bus_station.bus_stop.bus_stop_not_found import BusStopNotFound
 from bus_station.bus_stop.registration.supervisor.bus_stop_registration_supervisor import BusStopRegistrationSupervisor
 from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
 from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 
 S = TypeVar("S", bound=BusStop)
 
 
@@ -19,14 +21,16 @@
         self.__registration_supervisors = registration_supervisors
         self.__bus_stop_passenger_resolver = bus_stop_passenger_resolver
         self.__registered_bus_stops: Set[str] = set()
         self.__bus_stop_name_id_mapping: Dict[str, str] = {}
 
     def register(self, bus_stop_id: str) -> None:
         bus_stop = self._bus_stop_resolver.resolve(bus_stop_id)
+        if bus_stop is None:
+            raise BusStopNotFound(bus_stop_id)
         self.__add_bus_stop_name_mapping(bus_stop_id, bus_stop)
         self.__registered_bus_stops.add(bus_stop_id)
         self.__register_in_passenger_registry(bus_stop_id, bus_stop)
         self.__notify_registration(bus_stop_id)
 
     def __add_bus_stop_name_mapping(self, bus_stop_id: str, bus_stop: BusStop) -> None:
         self.__bus_stop_name_id_mapping[bus_stop.bus_stop_name()] = bus_stop_id
@@ -40,14 +44,16 @@
             return
 
         for supervisor in self.__registration_supervisors:  # pyre-ignore[16]
             supervisor.on_register(bus_stop_id)
 
     def unregister(self, bus_stop_id: str) -> None:
         bus_stop = self._bus_stop_resolver.resolve(bus_stop_id)
+        if bus_stop is None:
+            raise BusStopNotFound(bus_stop_id)
         self.__remove_bus_stop_name_mapping(bus_stop)
         self.__registered_bus_stops.remove(bus_stop_id)
         self.__unregister_in_passenger_registry(bus_stop_id)
         self.__notify_unregistration(bus_stop_id)
 
     def __remove_bus_stop_name_mapping(self, bus_stop: BusStop) -> None:
         del self.__bus_stop_name_id_mapping[bus_stop.bus_stop_name()]
```

### Comparing `bus_station-6.1.1/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py` & `bus_station-6.1.2/src/bus_station/bus_stop/registration/supervisor/bus_stop_address_registration_supervisor.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py` & `bus_station-6.1.2/src/bus_station/bus_stop/resolvers/in_memory_bus_stop_resolver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from typing import Dict, Optional, TypeVar
+from typing import Dict, Optional
 
 from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
 from bus_station.shared_terminal.fqn import resolve_fqn
 
-S = TypeVar("S", bound=BusStop)
 
-
-class InMemoryBusStopResolver(BusStopResolver[S]):
+class InMemoryBusStopResolver(BusStopResolver):
     def __init__(self):
-        self.__bus_stops: Dict[str, S] = {}
+        self.__bus_stops: Dict[str, BusStop] = {}
 
-    def add_bus_stop(self, bus_stop: S) -> None:
+    def add_bus_stop(self, bus_stop: BusStop) -> None:
         fqn = resolve_fqn(bus_stop)
         self.__bus_stops[fqn] = bus_stop
 
-    def resolve(self, bus_stop_id: str) -> Optional[S]:
+    def resolve(self, bus_stop_id: str) -> Optional[BusStop]:
         return self.__bus_stops.get(bus_stop_id)
```

### Comparing `bus_station-6.1.1/src/bus_station/bus_stop/resolvers/pypendency_bus_stop_resolver.py` & `bus_station-6.1.2/src/bus_station/bus_stop/resolvers/yandil_bus_stop_resolver.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,29 @@
-from typing import Optional, TypeVar
+from importlib import import_module
+from typing import Optional, Type
 
-from pypendency.container import Container
+from yandil.container import Container, default_container  # pyre-ignore[21]
 
 from bus_station.bus_stop.bus_stop import BusStop
 from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
 
-S = TypeVar("S", bound=BusStop)
 
+class YandilBusStopResolver(BusStopResolver):
+    def __init__(self, container: Optional[Container] = None):  # pyre-ignore[11]
+        self.__container = container or default_container
+
+    def resolve(self, bus_stop_id: str) -> Optional[BusStop]:
+        bus_stop_class = self.__get_class_from_fqn(bus_stop_id)
+        if bus_stop_class is None:
+            return None
 
-class PypendencyBusStopResolver(BusStopResolver[S]):
-    def __init__(self, pypendency_container: Container):
-        self.__pypendency_container = pypendency_container
+        resolved_bus_stop = self.__container[bus_stop_class]
 
-    def resolve(self, bus_stop_id: str) -> Optional[S]:
-        resolved_instance = self.__pypendency_container.get(bus_stop_id)
-        if resolved_instance is None:
-            return None
-        if not issubclass(resolved_instance.__class__, BusStop):
+        if not issubclass(resolved_bus_stop.__class__, BusStop):
             raise TypeError(f"Instance resolved from {bus_stop_id} is not a valid BusStop")
-        return resolved_instance  # type: ignore
+
+        return resolved_bus_stop
+
+    def __get_class_from_fqn(self, fqn: str) -> Type:
+        module_name, class_qualname = fqn.rsplit(".", 1)
+        module = import_module(module_name)
+        return getattr(module, class_qualname)
```

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/distributed/kombu_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/memory_queue_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus/asynchronous/threaded_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/json_rpc_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/distributed/rpyc_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus/synchronous/sync_command_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/json_rpc_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/kombu_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/memory_queue_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py` & `bus_station-6.1.2/src/bus_station/command_terminal/bus_engine/rpyc_command_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/command_handler_registry.py` & `bus_station-6.1.2/src/bus_station/command_terminal/command_handler_registry.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from functools import partial
 from typing import List, Optional
 
 from bus_station.bus_stop.registration.bus_stop_registry import BusStopRegistry
 from bus_station.bus_stop.registration.supervisor.bus_stop_registration_supervisor import BusStopRegistrationSupervisor
 from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
 from bus_station.command_terminal.command_handler import CommandHandler
+from bus_station.command_terminal.handler_not_found_for_command import HandlerNotFoundForCommand
 from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
 
 
 class CommandHandlerRegistry(BusStopRegistry[CommandHandler]):
     def __init__(
         self,
@@ -24,8 +25,12 @@
 
     def get_handler_from_command(self, command_name: str) -> Optional[CommandHandler]:
         command_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(command_name)
         if len(command_handler_ids) == 0:
             return None
 
         command_handler_id = next(iter(command_handler_ids))
-        return self._bus_stop_resolver.resolve(command_handler_id)
+        resolved_command_handler = self._bus_stop_resolver.resolve(command_handler_id)
+
+        if not isinstance(resolved_command_handler, CommandHandler):
+            raise HandlerNotFoundForCommand(command_name)
+        return resolved_command_handler
```

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/json_rpc_command_server.py` & `bus_station-6.1.2/src/bus_station/command_terminal/json_rpc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/middleware/command_middleware.py` & `bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/middleware/command_middleware_receiver.py` & `bus_station-6.1.2/src/bus_station/command_terminal/middleware/command_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py` & `bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/logging_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py` & `bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/timing_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py` & `bus_station-6.1.2/src/bus_station/command_terminal/middleware/implementations/tracking_command_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/command_terminal/rpyc_command_server.py` & `bus_station-6.1.2/src/bus_station/command_terminal/rpyc_command_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py` & `bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/distributed/kombu_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py` & `bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/memory_queue_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py` & `bus_station-6.1.2/src/bus_station/event_terminal/bus/asynchronous/threaded_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py` & `bus_station-6.1.2/src/bus_station/event_terminal/bus/synchronous/sync_event_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py` & `bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/kombu_event_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py` & `bus_station-6.1.2/src/bus_station/event_terminal/bus_engine/memory_queue_event_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/event_consumer_registry.py` & `bus_station-6.1.2/src/bus_station/event_terminal/event_consumer_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/middleware/event_middleware.py` & `bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/middleware/event_middleware_receiver.py` & `bus_station-6.1.2/src/bus_station/event_terminal/middleware/event_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py` & `bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/logging_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py` & `bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/timing_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py` & `bus_station-6.1.2/src/bus_station/event_terminal/middleware/implementations/tracking_event_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/memory_queue_passenger_worker.py` & `bus_station-6.1.2/src/bus_station/passengers/memory_queue_passenger_worker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/passenger.py` & `bus_station-6.1.2/src/bus_station/passengers/passenger.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/passenger_kombu_consumer.py` & `bus_station-6.1.2/src/bus_station/passengers/passenger_kombu_consumer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/passenger_mapper.py` & `bus_station-6.1.2/src/bus_station/passengers/passenger_mapper.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/passenger_registry.py` & `bus_station-6.1.2/src/bus_station/passengers/passenger_registry.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/passenger_resolvers.py` & `bus_station-6.1.2/src/bus_station/passengers/passenger_resolvers.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/reception/passenger_middleware_receiver.py` & `bus_station-6.1.2/src/bus_station/passengers/reception/passenger_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/reception/passenger_receiver.py` & `bus_station-6.1.2/src/bus_station/passengers/reception/passenger_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/serialization/passenger_json_deserializer.py` & `bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_deserializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/passengers/serialization/passenger_json_serializer.py` & `bus_station-6.1.2/src/bus_station/passengers/serialization/passenger_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py` & `bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/json_rpc_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py` & `bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/distributed/rpyc_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py` & `bus_station-6.1.2/src/bus_station/query_terminal/bus/synchronous/sync_query_bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py` & `bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/json_rpc_query_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py` & `bus_station-6.1.2/src/bus_station/query_terminal/bus_engine/rpyc_query_bus_engine.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/json_rpc_query_server.py` & `bus_station-6.1.2/src/bus_station/query_terminal/json_rpc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py` & `bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/logging_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py` & `bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/timing_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py` & `bus_station-6.1.2/src/bus_station/query_terminal/middleware/implementations/tracking_query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/middleware/query_middleware.py` & `bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/middleware/query_middleware_receiver.py` & `bus_station-6.1.2/src/bus_station/query_terminal/middleware/query_middleware_receiver.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/query_handler.py` & `bus_station-6.1.2/src/bus_station/query_terminal/query_handler.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/query_handler_registry.py` & `bus_station-6.1.2/src/bus_station/query_terminal/query_handler_registry.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from typing import List, Optional
 
 from bus_station.bus_stop.registration.bus_stop_registry import BusStopRegistry
 from bus_station.bus_stop.registration.supervisor.bus_stop_registration_supervisor import BusStopRegistrationSupervisor
 from bus_station.bus_stop.resolvers.bus_stop_resolver import BusStopResolver
 from bus_station.passengers.passenger_registry import passenger_bus_stop_registry
 from bus_station.passengers.passenger_resolvers import resolve_passenger_class_from_bus_stop
+from bus_station.query_terminal.handler_not_found_for_query import HandlerNotFoundForQuery
 from bus_station.query_terminal.query_handler import QueryHandler
 
 
 class QueryHandlerRegistry(BusStopRegistry[QueryHandler]):
     def __init__(
         self,
         bus_stop_resolver: BusStopResolver,
@@ -24,8 +25,12 @@
 
     def get_handler_from_query(self, query_name: str) -> Optional[QueryHandler]:
         query_handler_ids = passenger_bus_stop_registry.get_bus_stops_for_passenger(query_name)
         if len(query_handler_ids) == 0:
             return None
 
         query_handler_id = next(iter(query_handler_ids))
-        return self._bus_stop_resolver.resolve(query_handler_id)
+        resolved_query_handler = self._bus_stop_resolver.resolve(query_handler_id)
+
+        if not isinstance(resolved_query_handler, QueryHandler):
+            raise HandlerNotFoundForQuery(query_name)
+        return resolved_query_handler
```

### Comparing `bus_station-6.1.1/src/bus_station/query_terminal/rpyc_query_server.py` & `bus_station-6.1.2/src/bus_station/query_terminal/rpyc_query_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py` & `bus_station-6.1.2/src/bus_station/shared_terminal/broker_connection/connection_parameters/rabbitmq_connection_parameters.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/shared_terminal/bus.py` & `bus_station-6.1.2/src/bus_station/shared_terminal/bus.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py` & `bus_station-6.1.2/src/bus_station/shared_terminal/engine/runner/process_engine_runner.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/shared_terminal/factories/memory_queue_factory.py` & `bus_station-6.1.2/src/bus_station/shared_terminal/factories/memory_queue_factory.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/shared_terminal/json_rpc_server.py` & `bus_station-6.1.2/src/bus_station/shared_terminal/json_rpc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/shared_terminal/kafka_topic_creator.py` & `bus_station-6.1.2/src/bus_station/shared_terminal/kafka_topic_creator.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/shared_terminal/rpyc_server.py` & `bus_station-6.1.2/src/bus_station/shared_terminal/rpyc_server.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py` & `bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_model_tracking_map.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py` & `bus_station-6.1.2/src/bus_station/tracking_terminal/models/passenger_tracking_json_serializer.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py` & `bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/kafka_passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/src/bus_station/tracking_terminal/trackers/passenger_tracker.py` & `bus_station-6.1.2/src/bus_station/tracking_terminal/trackers/passenger_tracker.py`

 * *Files identical despite different names*

### Comparing `bus_station-6.1.1/PKG-INFO` & `bus_station-6.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bus-station
-Version: 6.1.1
+Version: 6.1.2
 Summary: A python bus station
 Author: DeejayRevok
 Author-email: seryi_one@hotmail.com
 Requires-Python: >=3.10.0,<3.11.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: confluent-kafka (>=2.1.1,<3.0.0)
```

