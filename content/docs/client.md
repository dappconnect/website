# Client

In it's simplest form a client is a Javascript enabled website that interacts with the host. The interaction is achieved through message passing.


## Identify the Host

  if (navigator.userAgent.indexOf('dappConnect')>=0) {

  }

The userAgent string should be of the form:

HostAppName iOS|Android dappConnect


## Getting Started


    function responseHandler(context: {messageId : string, path: string,},  data: any) {

    }

    window.addEventListener("dappConnectLoaded", function() {
      // window.dappConnect is now available

      // const hasFeatureX = window.dappConnect.features.X;

      window.dappConnect.addResponseHandler(responseHandler);
      const messageId = window.dappConnect.request('/feature/path',{some: 'data'});
    });



