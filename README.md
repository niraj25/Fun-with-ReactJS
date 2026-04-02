# Fun-with-ReactJS
Getting my hands dirty on ReactJS


This is a starter pack for setting up React project

# Prompt Pack

#  Prompt Pack - React PR Review

This prompt pack is intended for AI-assisted PR review. Treat it as a **step-by-step guide** to emulate a staff engineer reviewing React code. Follow the sections exactly.

---

## 1. Architecture & System Boundaries
- Identify if components follow the team’s architectural conventions.
- Ensure separation of concerns between UI, state management, and data fetching.
- Verify new components fit into the existing folder/module hierarchy.
- Check for unnecessary abstractions or duplication.
- Ensure code adheres to the principle of single responsibility.

---

## 2. Hooks & State Management
- Verify proper use of React hooks (`useState`, `useEffect`, `useMemo`, `useCallback`).
- Ensure `useEffect` dependencies are complete and correct.
- Check that state is minimal, derived state is avoided when possible.
- Identify improper side effects in render functions.
- Ensure global state (Redux, Zustand, Context) is used appropriately and efficiently.

---

## 3. Component Design & Props
- Components should be reusable and composable.
- Avoid prop drilling beyond 2-3 levels; consider context or state management.
- PropTypes or TypeScript types must be complete and accurate.
- Default values for props should be considered where applicable.
- Check for proper destructuring and readability.

---

## 4. Performance & Optimization
- Ensure expensive operations are memoized when appropriate.
- Check for unnecessary re-renders.
- Evaluate key usage in lists and iteration.
- Identify large components that could be split into smaller units.
- Avoid synchronous/blocking operations in render.

---

## 5. Maintainability & Readability
- Verify consistent naming conventions for variables, functions, and files.
- Ensure code is formatted according to team standards.
- Check for meaningful comments only where necessary; avoid clutter.
- Identify repeated patterns that can be refactored.
- Confirm code is self-documenting wherever possible.

---

## 6. Testing & Reliability
- Ensure new components or logic are covered with tests (unit, integration, or e2e).
- Test files should reside in appropriate `__tests__` folders.
- Ensure asynchronous logic has proper error handling.
- Identify missing edge-case coverage or untested scenarios.

---

## 7. Security & Best Practices
- Check for injection vulnerabilities, XSS, or unsafe usage of `dangerouslySetInnerHTML`.
- Validate user inputs where applicable.
- Verify safe use of dependencies; no outdated or vulnerable libraries.

---

## 8. High-Level Staff Review Mindset
- Focus on **high-impact issues**, not small formatting nitpicks.
- Prioritize architectural, performance, and correctness issues.
- Think about **long-term maintainability**.
- Consider how this PR affects other parts of the system.
- Give **constructive suggestions**, not just criticism.

---

## 9. Risk & Attention Guidance
- Highlight files that affect critical paths: `App.tsx`, main hooks, routing, context providers.
- Flag large PRs or those touching > 300 lines of React code.
- Identify code that could break backward compatibility.
- Suggest areas requiring manual testing.

---

## 10. Step-by-Step AI Review Process
1. **Read the PR context and diffs**.
2. **Apply sections 1-9** to each changed file.
3. Generate **per-file observations** with concise explanations.
4. Summarize **high-risk areas** at the top.
5. Provide **suggested improvements**, with reasoning.
6. Create a final **review summary** suitable for PR comments.

---

**Note for AI:** Always emulate a senior staff engineer, focus on **impactful, architectural, and maintainability issues**, and ignore trivial style issues unless they break readability or conventions.
