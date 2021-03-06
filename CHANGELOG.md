# Change Log
All notable changes to this project will be documented in this file. This change log follows the conventions of [keepachangelog.com](http://keepachangelog.com/).

## [Unreleased]

## 0.5.0 (2020-12-14)

- Works against flow-storm-debugger > 0.6.0 
- Encode data as transit and send it in baches of 500ms for better performance
- Don't connect if we already have a connection

## 0.4.2 (2020-11-27)

- Resolve add-tap with resolve so flow-storm can be used with older versions of clojure
- Do patches value serialization
- Fix ref-init-trace value serialization

## 0.4.1 (2020-11-20)

- Add :timestamp to all traces (but binding ones)
- Add tap tracing
- Add :ignore-keys to trace-ref opts map
- Don't trace empty patches

## 0.4.0 (2020-11-17)

- Implemented ref-tracing via :flow-storm/ref-init-trace and :flow-storm/ref-trace

## 0.3.2 (2020-11-06)

- Fix multi arity fn support for cljs
- Multimethods trace support
- Implements trace-var, untrace-var 
- Fix #5 Instrumented code of [& args] doesn't compile

## 0.3.1 (2020-10-31)

- Add exception names in error messages
- Fix #9, no tracing inside case in ClojureScript

## 0.3.0 (2020-10-30)

- Add exception tracing (#2)
- Add #ztrace for tracing with flow-id 0

## 0.2.7 (2020-10-23)

- Adding `:protocol` option to connect config map
- Upgrading com.taoensso/sente to 1.16.0
- Serialize init-trace args-vec for fixing the "bad package" error

## 0.2.6 (2020-10-16)
