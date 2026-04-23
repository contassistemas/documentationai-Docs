# Common errors from CloudStack

## 504 Gateway Timeout

This error occurs when the CloudStack API takes too long to respond. It can happen due to:

- Long-running operations (like deploying a VM with many steps)
- Network connectivity issues between the API and the hypervisor
- High load on the CloudStack management server

### Solutions:

1. **Increase timeout settings** in your CloudStack configuration
2. **Check network connectivity** between the API and hypervisor
3. **Monitor system resources** on the management server
4. **Break down large operations** into smaller, sequential tasks
5. **Implement retry logic** with exponential backoff in your applications