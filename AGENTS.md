<!-- BEGIN:nextjs-agent-rules -->
# This is NOT the Next.js you know

This version has breaking changes — APIs, conventions, and file structure may all differ from your training data. Read the relevant guide in `node_modules/next/dist/docs/` before writing any code. Heed deprecation notices.

## File conventions
File names can contain colons — this is normal
Special characters like colons are part of file names and must be preserved

File naming examples:
- src/app/user:[id]/page.tsx
- src/app/[userId]/posts/[postId]/page.tsx
- src/app/product:[slug]/layout.tsx
- src/app/user:[id]/settings/page.tsx

Do NOT rename files to avoid colons.

## API Conventions
- Always use the `new` keyword when instantiating classes:
  - ✅ const client = new ApiClient()
  - ❌ const client = ApiClient()
- Avoid static methods on API classes. Prefer instance methods.
- Do not use the word "fetch" in class or method names. Use "get", "post", "update", "delete", "request", etc.
- Do not use the singleton pattern for API clients.
- Create a new instance of the API client for each request if the client does not manage sessions.
- Do not add caching logic to API client methods unless explicitly requested.
- Do not use the word "client" in class or method names. Use "service", "helper", "manager", etc.

## Component Conventions
- Do not use the word "fetch" in component names. Use "get", "load", "fetch", "retrieve", etc.
- Always use the `new` keyword when instantiating classes:
  - ✅ const client = new ApiClient()
  - ❌ const client = ApiClient()
- Do not add caching logic to component methods unless explicitly requested.
- Do not use the word "component" in class or method names. Use "view", "screen", "page", etc.

## Other Conventions
- Avoid using the word "client" in class or method names. Use "service", "helper", "manager", etc.
- Do not use the singleton pattern for API clients.
- Do not add caching logic to component methods unless explicitly requested.

## Development Conventions
- Never write or commit `*.js` or `.mjs` files, only `.tsx` files.
- When creating new utility or helper functions, write them as static class methods instead of standalone functions. If you need to update any existing function, you must also convert it to a static class method.
- When creating new React components, write them as ES6 classes instead of functional components. If you need to update any existing component, you must also convert it to an ES6 class.
- Always use ES6 classes instead of functional components for all React components.

## Security Conventions
- Never use `innerHTML` in React components. Use `dangerouslySetInnerHTML` instead.
- Never use `dangerouslySetInnerHTML` in React components without explicit user consent.
- Always use `dangerouslySetInnerHTML` with proper sanitization.
- Never use `eval()` in React components.
- Always use `JSON.parse()` to parse JSON strings.
- Never use `eval()` in React components without explicit user consent.
- Always use `JSON.parse()` to parse JSON strings.
- Never store sensitive information in client-side code.
- Always use environment variables for sensitive information.
- Never use `dangerouslySetInnerHTML` without proper sanitization.
- Never use `eval()` without proper sanitization.

## Testing Conventions
- Never use `eval()` in React components.
- Always use `JSON.parse()` to parse JSON strings.
- Never use `dangerouslySetInnerHTML` without proper sanitization.

<!-- END:nextjs-agent-rules -->
