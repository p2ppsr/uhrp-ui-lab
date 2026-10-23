# NanoStore UI

Upload and Download Content

## License

The license for the code in this repository is the Open BSV License.


## October2026 Node build security maintenance

Retained build tooling uses Node22.23.4 and the existing frozen dependency lock.
Historical npm6 peer resolution is retained. PR CI verifies the patched native
Node/Brotli runtime and builds the retained source; registry fetches are bounded
and failures remain failures. Application dependency versions and browser
contracts are unchanged. The obsolete Cloud Run deployment is retained only as
a non-executable reference at `docs/legacy-cloud-run-deploy.yaml.txt`. This source
update cannot recreate that legacy Cloud Run service. A working build does not
establish application or production-restoration acceptance.
