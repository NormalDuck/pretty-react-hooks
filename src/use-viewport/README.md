## 🪝 `useViewport`

```ts
function useViewport(listener?: (viewport: Vector2) => void): Roact.Binding<Vector2>;
```

Returns a binding to the size of the viewport.

If a listener is provided, it will be called when the viewport changes and once on mount.

### 📕 Parameters

-   `listener` - An optional listener to be called when the viewport size changes.

### 📗 Returns

-   The size of the viewport in pixels.

### 📘 Example

```tsx
export default function Component() {
	const viewport = useViewport();
	const textSize = viewport.map((size) => {
		return math.min(size.X / 1920, size.Y / 1080) * 14;
	});

	return <text TextSize={textSize} />;
}
```
