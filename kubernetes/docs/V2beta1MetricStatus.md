# Kubernetes::V2beta1MetricStatus

## Properties
Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**object** | [**V2beta1ObjectMetricStatus**](V2beta1ObjectMetricStatus.md) | object refers to a metric describing a single kubernetes object (for example, hits-per-second on an Ingress object). | [optional] 
**pods** | [**V2beta1PodsMetricStatus**](V2beta1PodsMetricStatus.md) | pods refers to a metric describing each pod in the current scale target (for example, transactions-processed-per-second).  The values will be averaged together before being compared to the target value. | [optional] 
**resource** | [**V2beta1ResourceMetricStatus**](V2beta1ResourceMetricStatus.md) | resource refers to a resource metric (such as those specified in requests and limits) known to Kubernetes describing each pod in the current scale target (e.g. CPU or memory). Such metrics are built in to Kubernetes, and have special scaling options on top of those available to normal per-pod metrics using the \&quot;pods\&quot; source. | [optional] 
**type** | **String** | type is the type of metric source.  It will match one of the fields below. | 


