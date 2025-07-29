In this directory are patches for [snircd](https://github.com/quakenet/snircd).<br>
<br>
**Following patches are available:**<br>

**IRCv3-capabilities.patch** - Comprehensive IRCv3 capabilities implementation for snircd, adding modern IRC protocol support including:
- **SASL Authentication**: Full SASL support via iauthd integration with proper authentication flow and account management
- **Message Tags**: Complete message-tags capability with typing indicators (@+typing=active, @+typing=paused, @+typing=done) and draft/typing tags
- **Account Notifications**: account-notify capability for real-time account status updates
- **Away Notifications**: away-notify capability for instant away status changes
- **Extended Join**: extended-join capability providing account information in JOIN messages
- **Change Host**: chghost capability for real-time hostname change notifications
- **Echo Message**: echo-message capability allowing clients to see their own messages
- **Invite Notify**: invite-notify capability for channel invitation notifications
- Improved capability negotiation system with proper CAP LS/REQ/ACK/END handling
- Enhanced authentication system integration with comprehensive SASL mechanisms
- Full compatibility with modern IRC clients supporting IRCv3 standards

**configure.patch** - Fixes critical MAXCONNECTIONS configuration issues by implementing a hard limit cap:
- Sets maximum client connections to 262,168 (NN_MAX_CLIENT_P) to prevent system resource exhaustion
- Prevents potential crashes or performance issues when systems attempt to set unlimited or excessively high connection limits
- Ensures stable operation under high-load scenarios by enforcing reasonable connection boundaries
- Addresses configuration edge cases where ulimit values could exceed safe operational limits<br>
