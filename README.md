# Pinning using IPFS cli

to add piniata gateway dont woory about the domain(still havent figured out why i even bought it)
the api endpoint is the same I guesse and the jwt coonects to my domain (i think)

```
ipfs pin remote service add pinata https://api.pinata.cloud/psa YOUR_JWT
```

To pin a CID to Pinata under a human-readable name:
```
ipfs pin remote add --service=pinata --name=war-and-peace.txt bafybeib32tuqzs2wrc52rdt56cz73sqe3qu2deqdudssspnu4gbezmhig4
```

To list successful pins:
```
ipfs pin remote ls --service=pinata
```

To list pending pins:
```
ipfs pin remote ls --service=pinata --status=queued,pinning,failed
```
