⚠️ This project has moved to [ably/test-observability-action](https://github.com/ably/test-observability-action).

# Test Observability Action

An action to push junit files to Ably's test observability server.

# Inputs

- server-url - url to publish results to
- server-auth - auth key for server
- path - path to look for *.junit files

# Example

```
      - name: Upload test results
        if: always()
        uses: ably-labs/test-observability-action@main
        with:
          server-url: 'https://test-observability.herokuapp.com'
          server-auth: ${{ secrets.TEST_OBSERVABLILITY_SERVER_AUTH }}
          path: '.'
```
