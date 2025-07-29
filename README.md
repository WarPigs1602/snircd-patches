# snircd-patches

In this directory are patches for [snircd](https://github.com/quakenet/snircd).

## Available Patches

### IRCv3-capabilities.patch

This patch extends snircd to add support for several IRCv3 capabilities, improving interoperability with modern IRC clients and networks.  
Notable features included:
- **SASL authentication support** (over iauthd): Enables secure client authentication using the SASL mechanism.
- **message-tags**: Allows tags to be attached to messages, for example to show who is typing.
- **Additional IRCv3 capabilities**:
  - `account-notify`
  - `away-notify`
  - `chghost`
  - `echo-message`
  - `extended-join`
  - `invite-notify`
- Adapts the capability advertisement and feature negotiation to modern standards.

See the patch for full details and implementation.

---

### configure.patch

Resolves issues with the `MAXCONNECTIONS` configuration in snircd's build process:
- Dynamically determines the system's maximum number of allowed open connections.
- Ensures the configured value does not exceed a defined upper limit (`NN_MAX_CLIENT_P`).
- Prevents server instability or crashes due to overly high connection configuration.

This patch is recommended to ensure reliable operation on systems with large resource limits.

---

For more information or to view these patches, see the repository: [WarPigs1602/snircd-patches](https://github.com/WarPigs1602/snircd-patches).
