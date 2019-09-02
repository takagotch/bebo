### bebo
---
https://github.com/bebo

#### bebo-capture
https://github.com/bebo/bebo-capture

```cc
// bebo-capture-svc/BeboCaptureFactory.cpp

#include "Bebo"
#include "BeboCapture.h"

HRESULT __stdcall CBeboCaptureFactory::CreateInstance(IUnknown* pUnknownOuter,
    const IID& iid,
    void** ppv)
{
  if (pUnknownOuter != NULL)
  {
    return CLASS_E_NOAGGREGATION;
  }
  
  if (pUnknownOuter != NULL)
  {
    return CLASS_E_NOAGGREGATION;
  }
  
  CBeboCapture* pObject = new CBeboCapture;
  if (pObject == NULL)
  {
    return E_OUTOFMEMORY;
  }
  
  return pObject->QueryInterface(iid, ppv);
}

HRESULT __stdall CBeboCaptureFactory::LockServer(BOOK bLock)
{
  return E_NOTIMPL;
}
```

```
```

```
```


