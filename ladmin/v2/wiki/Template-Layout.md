### Guest Layout
```html
<x-ladmin-guest-layout>
  
  <x-slot name="metaTitle">Meta Page Title</x-slot>

  @push('before-style')
    <!-- ... -->
  @endpush
  <x-slot name="styles">
    <!-- <link href="custom.css" rel="stylesheet" /> -->
  </x-slot>
  @push('after-style')
    <!-- ... -->
  @endpush

  <!-- Content here -->

  @push('before-script')
    <!-- ... -->
  @endpush
  <x-slot name="scripts">
    <!-- <script src="custom.js" ></script> -->
  </x-slot>
  @push('after-script')
    <!-- ... -->
  @endpush

</x-ladmin-guest-layout>
```

## Auth Layout

```html
<x-ladmin-auth-layout>

  <x-slot name="title">Page Title</x-slot>

  <!-- Follow guest layout for slots & stacks -->
  
</x-ladmin-auth-layout>
```