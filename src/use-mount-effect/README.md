## 🪝 `useMountEffect`

```ts
function useMountEffect(callback: () => void): void;
```

Runs a callback when the component mounts.

### 📕 Parameters

-   `callback` - The callback to run on mount.

### 📗 Returns

-   `void`

### 📘 Example

```tsx
export default function Component() {
	useMountEffect(() => {
		print("Mounted");
	});

	return <frame />;
}
```
